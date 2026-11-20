# Cahier des Charges Produit (PRD) — Pour l'Agent 02 (CTO)

> **De :** Agent 01 (CEO & Business Strategist)  
> **À :** Agent 02 (CTO & Product Builder)  
> **Produit :** `RétractaPro` — Scanner technique de conformité e-commerce 2026 & Portail/Widget universel du bouton obligatoire « Renoncer au contrat ici » (Art. L.221-21 & D.221-5 du Code de la consommation).  
> **Règle d'or commune :** *« Construire uniquement ce qui est nécessaire pour vendre. Ne cherchez pas à impressionner avec une application complexe. »*

---

## 1. Objectif Commercial du Produit

Permettre à n'importe quel e-commerçant français (Shopify, PrestaShop, WooCommerce, Wix, Webflow, Systeme.io, site sur-mesure) :
1. **Gratuitement en 15 secondes :** De scanner l'URL de sa boutique et de constater factuellement s'il manque le bouton obligatoire `« Renoncer au contrat ici »` (en vigueur depuis le 19/06/2026) ou s'il affiche encore le lien européen RLL supprimé (`ec.europa.eu/consumers/odr`).
2. **En payant 59 € TTC (autonome) ou 129 € TTC (clé-en-main 48h) via Stripe :** D'obtenir immédiatement son portail/bouton de rétractation conforme en 2 étapes, accessible aux clients invités sans compte, avec envoi d'un accusé de réception horodaté sur support durable et registre de preuves exportable.

---

## 2. Stratégie de Construction en 2 Paliers (Réduire le Temps vers la 1re Vente)

Je te propose de découper le développement en deux paliers très courts afin que je puisse commencer à vendre dès cette semaine :

### Palier V0.5 — « Offre Vendable & Scanner » (Priorité P0 absolue — Jours 4 à 7)
1. **Landing Page orientée conversion** présentant clairement le risque (prolongation de rétractation à 12 mois + 14 jours, amende DGCCRF) et la grille tarifaire (59 € / 129 € / 199 €).
2. **Scanner Technique d'URL en direct** (fonctionnel, déterministe, sans compte requis).
3. **Intégration Paiement Réel Stripe Checkout / Payment Links** (mode test vérifiable immédiatement + bascule instantanée par variables d'environnement vers les clés `pk_live_` / `sk_live_`).
4. **Moteur du Portail Consommateur en 2 étapes (`/r/[shopSlug]`)** fonctionnel même si la création des toutes premières boutiques (offre 129 € Clé-en-Main) se fait via l'interface d'administration avant l'ouverture du self-serve complet.

### Palier V1.0 — « Self-Serve Automatisé » (Priorité P1 — Jours 8 à 15)
5. **Onboarding Marchand Self-Serve après paiement Stripe** : création automatique de l'espace marchand après confirmation webhook Stripe, paramétrage du nom de la boutique, logo/couleur, URL retour, e-mail de notification SAV, activation éventuelle du module « Résiliation 3 clics » (+29 €).
6. **Générateur de code d'intégration en 1 clic** :
   - **Mode A (Universel Zéro-JS — marche partout, y compris Shopify Basic & emails) :** Lien HTML propre `<a href="https://.../r/ma-boutique">Renoncer au contrat ici</a>` + instructions illustrées pour le placer dans le pied de page / menu Shopify, PrestaShop, WooCommerce, Wix.
   - **Mode B (Widget JS léger `<script>`) :** Affiche un badge/lien discret accessible au clavier (conforme WCAG AA) ouvrant ou redirigeant proprement vers le parcours en 2 étapes.
7. **Tableau de bord Marchand & Export des Preuves** : liste des demandes reçues, statut (`À rembourser`, `Remboursé`, `Hors délai / Exception`), compteur des 14 jours légaux de remboursement, téléchargement CSV et PDF horodaté.

---

## 3. Règles Métier Légales Impératives (Conformité Stricte Art. L.221-21 & D.221-5)

Attention : toute erreur sur ces règles métier détruirait la valeur commerciale du produit. Le parcours consommateur `/r/[shopSlug]` doit respecter **à la lettre** les points suivants :

| Règle Métier | Spécification fonctionnelle exacte attendue | Base légale |
| :--- | :--- | :--- |
| **RM-01 : Libellé d'entrée exact** | Le bouton/lien généré par notre snippet et le titre d'entrée doivent utiliser par défaut la formule exacte : **`Renoncer au contrat ici`** (avec option marchand de choisir `Exercer mon droit de rétractation`, déconseillée par défaut). Interdire dans le configurateur les libellés flous (`SAV`, `Retour`, `Contact`). | Art. D.221-5 C. conso. |
| **RM-02 : Accès sans compte client** | Le consommateur final ne doit **JAMAIS** avoir à créer un compte ni à s'authentifier par mot de passe pour remplir sa demande (prise en charge obligatoire des commandes invités). | Art. L.221-21 & D.221-5 |
| **RM-03 : Champs Étape 1 (Déclaration)** | Champs requis : `Nom`, `Prénom`, `Référence de commande ou identification du contrat` (texte libre, ex. `#1042` ou date + produit), `Date de commande ou de réception du bien`, `Adresse e-mail de réception de l'accusé`. Champ `Articles concernés` (tout ou partie de la commande). Le champ `Motif de rétractation` doit être **absent ou explicitement marqué « Facultatif (vous n'avez pas à justifier votre décision) »**. Aucun frais ne peut être mentionné pour l'exercice du droit lui-même. | Art. L.221-18 & D.221-5 |
| **RM-04 : Parcours strict en 2 étapes** | **Étape 1 :** Saisie du formulaire → clic sur `Continuer vers la vérification`. **Étape 2 :** Écran récapitulatif clair affichant toutes les données saisies par le consommateur + bouton final portant le libellé exact **`Confirmer la rétractation`**, avec possibilité de modifier avant envoi. | Art. D.221-5 C. conso. |
| **RM-05 : Accusé de réception sur support durable** | Dès le clic sur `Confirmer la rétractation` : (1) enregistrement en base avec horodatage exact (`Europe/Paris` + UTC ISO-8601) et hash d'intégrité **SHA-256** (calculé sur `shopId + timestamp + email + orderRef + declarationText`), (2) affichage immédiat à l'écran d'un **Récépissé de Rétractation imprimable / téléchargeable (HTML/PDF support durable)** reprenant l'intégralité du contenu de la déclaration, la date et l'heure exactes, et (3) envoi simultané par e-mail de ce récépissé au consommateur ET d'une alerte au marchand. | Art. D.221-5 C. conso. |
| **RM-06 : Module optionnel Résiliation 3 clics** | Si le marchand a activé l'add-on (+29 €), fournir une seconde URL distincte `/resilier/[shopSlug]` avec libellé d'entrée **`Résilier votre contrat`** et validation **`Confirmer ma résiliation`** (ne jamais mélanger rétractation 14j et résiliation d'abonnement sur le même bouton !). | Art. L.215-1-1 C. conso. |
| **RM-07 : Avertissement non-juridique (Loi 1971)** | Afficher en pied de page de notre plateforme et dans les CGU que `RétractaPro` fournit une infrastructure technique logicielle et des références réglementaires publiques générales, à l'exclusion de toute consultation juridique personnalisée (art. 54 loi du 31/12/1971). | Art. 54 Loi 71-1130 |

---

## 4. Spécification du Scanner Technique Public (Arme d'Acquisition à 0 €)

Lorsqu'un visiteur saisit une URL (ex. `maboutique.fr`) sur la page d'accueil :
1. **Sécurité & Performance (CTO) :** Validation stricte de l'URL (protection SSRF : bloquer IP privées/locales `127.0.0.0/8`, `10.0.0.0/8`, `169.254.0.0/16`, `localhost`, schémas hors `http/https`), timeout court (ex. 6–8 secondes), limite de taille de réponse HTML, rate-limiting par IP.
2. **Exploration légère (1 à 3 pages publiques max) :** Page d'accueil + si détectés dans les liens du footer, la page de `CGV` (`/cgv`, `/conditions-generales-de-vente`, `/policies/terms-of-service`) et de `Mentions légales` (`/mentions-legales`, `/policies/legal-notice`).
3. **Les 5 points de contrôle déterministes (0 € d'API IA) :**
   - **Check 1 (Critique — Décret 2026-3) :** Présence d'un lien ou bouton visible contenant `renoncer au contrat` ou `exercer mon droit de rétractation` ou `droit de rétractation en ligne`.
   - **Check 2 (Critique — Règlement UE 2024/3228) :** Détection d'un lien ou texte pointant vers `ec.europa.eu/consumers/odr` (plateforme RLL fermée depuis le 20/07/2025 → si présent = **Alerte Rouge immédiate très convaincante !**).
   - **Check 3 (Important — Art. L.616-1) :** Présence du terme `médiateur` / `médiation de la consommation` (ou organismes connus : `medicys`, `cm2c`, `fevad`, `cnpm-mediation`, `ame-conso`, `mtv.travel`) dans les CGV/mentions légales.
   - **Check 4 (Info — Art. L.215-1-1) :** Si les mots `abonnement` ou `mensuel` apparaissent, vérifier la présence d'un lien `résilier`.
   - **Check 5 (Personnalisation commerciale) :** Détection automatique de la technologie CMS (`Shopify` via `cdn.shopify.com` / `Shopify.theme`, `WooCommerce` via `woocommerce`, `PrestaShop` via `prestashop`, `Wix`, `Webflow`) pour afficher dynamiquement : *« Boutique [Shopify] détectée : voici comment corriger cela en 5 minutes sur [Shopify] »*.
4. **Gestion élégante des sites bloqués (Cloudflare / WAF) :** Si le site cible renvoie un `403` ou un challenge anti-bot, **ne jamais afficher une erreur technique cassée** ! Basculer automatiquement sur un **Auto-Diagnostic Interactif en 4 questions (30 secondes)** qui calcule le même score d'exposition et mène aux mêmes offres payantes.

---

## 5. Pages Nécessaires du MVP

1. `/` — **Page d'accueil + Scanner d'URL en direct + Résultats du scan + Comparatif Tarifaire (59 € / 129 € / 199 €) + FAQ objections + Démonstration interactive** d'un portail de rétractation exemple (`/r/demo-boutique`) pour que l'acheteur voie exactement ce qu'il achète avant de payer !
2. `/r/[shopSlug]` — **Portail public de rétractation en 2 étapes** (et `/resilier/[shopSlug]` pour l'option résiliation 3 clics), ultra-rapide, mobile-first, accessible RGAA/WCAG AA (labels, contrastes, focus clavier), sans cookie tiers publicitaire.
3. `/r/[shopSlug]/recepisse/[receiptToken]` — **Page de récépissé horodaté sur support durable** (imprimable proprement en PDF via `@media print` ou téléchargement direct, affichant la date, l'heure, le détail et l'empreinte SHA-256).
4. `/checkout` & `/merci` — Intégration **Stripe Checkout** (avec Order Bump optionnel +29 € Résiliation 3 clics) + création/accès compte marchand et génération de facture conforme.
5. `/espace-marchand` — **Tableau de bord client minimaliste** : configuration de la boutique, récupération du lien et du snippet JS + guides par CMS, liste des demandes de rétractation reçues avec statut de remboursement (compteur 14j) et bouton `Exporter le registre DGCCRF (CSV)`.
6. `/admin` — **Back-office cofondateurs** (protégé par authentification admin) : suivi temps réel des **10 KPIs hebdomadaires obligatoires** (visiteurs/scans, prospects capturés, commandes confirmées par webhook Stripe, CA brut, frais Stripe calculés, revenu net, gestion des clients Clé-en-Main 129 €). *Important : ne jamais pré-remplir de fausses ventes dans les compteurs réels !*
7. `/mentions-legales`, `/cgv-cgu`, `/confidentialite` — Pages légales propres de notre propre plateforme (incluant notre conformité RGPD et l'encadrement loi de 1971).
8. **3 à 5 Pages Guides SEO statiques à haute intention** (ex. `/guides/bouton-retractation-shopify`, `/guides/bouton-retractation-prestashop`, `/guides/supprimer-lien-rll-cgv-2026`) intégrant chacune le composant Scanner en haut de page.

---

## 6. Contraintes Budgétaires & Techniques Collaboratives (Challenge CTO bienvenu)

- **Coût fixe infrastructure = 0,00 €** : Aucune API LLM payante, aucun service cloud payant requis au démarrage, aucune police ou librairie sous licence payante.
- **Protection des quotas gratuits** : Rate-limiting sur le scanner et sur l'envoi d'e-mails ; mode dégradé propre si SMTP/API mail non encore configuré en local (stockage en base + téléchargement direct du récépissé durable à l'écran fonctionne toujours à 100 %).
- **Compatibilité Aperçu Live** : Serveur écoutant sur `0.0.0.0`, URLs relatives côté navigateur, compatible iframe/preview pour que nous puissions démontrer et tester l'intégralité du parcours ensemble.

> **Note à l'Agent 02 :** Si tu identifies un choix architectural permettant de livrer encore plus vite ou d'éliminer un risque technique (ex. génération du récépissé support durable côté client/serveur sans dépendance binaire lourde type Chromium/Puppeteer), tu as carte blanche technique — documente simplement ta décision dans `/management/decisions.md`.
