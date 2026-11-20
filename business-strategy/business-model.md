# Modèle Économique — `RétractaPro`

> **Principe directeur :** Rentabilité dès la première commande, zéro coût fixe au lancement, conformité juridique stricte sur le marché français.

---

## 1. Le Problème Résolu

Depuis le **19 juin 2026** (articles **L.221-21** et **D.221-5** du Code de la consommation issus de l'ordonnance n° 2026-2 et du décret n° 2026-3 du 5 janvier 2026), tout professionnel vendant en ligne des biens ou des services à des consommateurs en France (hors exceptions légales de l'art. L.221-28) doit proposer gratuitement sur son interface un parcours de rétractation en ligne respectant 6 exigences cumulatives :
1. Point d'entrée permanent, visible et directement accessible intitulé **« Renoncer au contrat ici »** (ou formule analogue dénuée d'ambiguïté).
2. Accès garanti **sans connexion obligatoire à un compte client** (prise en charge des achats invités).
3. Formulaire simple recueillant le nom/prénom, l'identification du contrat/commande et le moyen électronique de réception de l'accusé, **sans imposer de motif**.
4. Validation explicite en seconde étape par un bouton **« Confirmer la rétractation »**.
5. Transmission automatique d'un **accusé de réception horodaté sur support durable** (date, heure, contenu de la déclaration).
6. Cohérence technique avec le reste du pied de page marchand (retrait du lien européen RLL `ec.europa.eu/consumers/odr` supprimé le 20 juillet 2025, présence des coordonnées du médiateur de la consommation).

**Coût concret du problème non résolu pour un e-commerçant :**
- **Perte directe de marge par remboursements tardifs :** En l'absence de conformité, le délai légal de rétractation passe de **14 jours à 12 mois + 14 jours**. Deux remboursements forcés sur des paniers de 60 € coûtent déjà 120 € + frais logistiques.
- **Exposition aux contrôles en ligne DGCCRF :** Jusqu'à **15 000 €** (EI/micro-entreprise) et **75 000 €** (société) d'amende administrative (art. L.242-13).
- **Coût des solutions alternatives :** Payer un développeur freelance (300 € à 800 €) ou un SaaS récurrent comme `BackToMe` (25 € HT/mois soit 300 € HT/an).

---

## 2. Le Client Idéal (ICP — Ideal Customer Profile)

### Segment Primaire (Vente directe B2B — 80 % des ventes initiales)
- **Profil :** Fondateur/dirigeant de boutique e-commerce française (DNVB, commerce spécialisé, artisan vendant en ligne, créateur de formations/box B2C).
- **Taille :** 0 à 15 salariés, chiffre d'affaires annuel entre **30 000 € et 2 000 000 €** (cœur des 158 200 sites marchands français recensés par la FEVAD).
- ** Environnement technique :** **Shopify** (cible #1 prioritaire car checkout verrouillé et forte solvabilité), **PrestaShop**, **Wix**, **Webflow**, **Squarespace**, **Systeme.io**, ou **WooCommerce** géré sans développeur interne.
- **Comportement d'achat :** Décideur unique disposant de la carte bancaire de l'entreprise ; allergique aux nouveaux abonnements mensuels à 29 €/mois, mais prêt à payer immédiatement **59 € à 129 € en une fois** pour régler définitivement une obligation légale prouvée sur son propre site.

### Segment Secondaire Multiplicateur (B2B2B — 20 % des transactions, fort panier)
- **Profil :** Freelances web (Malt, collectifs Shopify/PrestaShop/WordPress) et petites agences digitales françaises gérant entre **5 et 50 boutiques clients**.
- **Motivation :** Acheter notre **Pack Agence 5 boutiques à 199 €** (soit **39,80 €/boutique**) et facturer une prestation globale de « Mise en conformité e-commerce 2026 » entre **150 € et 290 € HT** à chacun de leurs clients existants (marge immédiate pour le partenaire, zéro effort commercial unitaire pour nous).

---

## 3. La Solution Vendue & Proposition de Valeur

### Nature exacte du produit (Positionnement 100 % légal)
`RétractaPro` est un **logiciel technique d'interface e-commerce et de journalisation horodatée**, doublé d'un **scanner technique automatisé de pages publiques**.

> **Garde-fou légal impératif (Article 54 de la loi n° 71-1130 du 31 décembre 1971) :**  
> `RétractaPro` **ne délivre aucun conseil juridique personnalisé et ne rédige aucun acte sous seing privé sur mesure**. Nous fournissons exclusivement : (a) un composant technique logiciel implémentant le flux décrit à l'article D.221-5 du Code de la consommation, (b) un système informatique d'horodatage et d'envoi d'accusés de réception, (c) un outil de détection technique de balises/liens HTML publics, et (d) une documentation informative générale citant les textes officiels publics (Légifrance / Service-Public Entreprendre). Pour toute rédaction personnalisée de CGV, l'utilisateur est invité à consulter un avocat.

### Proposition de valeur unique
- **Rapide :** Opérationnel en **5 minutes** via un simple lien de pied de page `/r/votre-boutique` ou 1 ligne de script `<script>` compatible avec **100 % des CMS** (y compris Shopify Basic sans toucher au checkout).
- **Conforme techniquement au décret n° 2026-3 :** Libellés exacts `« Renoncer au contrat ici »` et `« Confirmer la rétractation »`, fonctionnement sans compte client (invités), motif facultatif, accusé de réception horodaté SHA-256 sur support durable + alerte marchand avec compte à rebours des 14 jours de remboursement.
- **Sans abonnement imposé :** Paiement unique clair (**59 € TTC** en autonome ou **129 € TTC** installé et testé par nos soins en 48h).

---

## 4. Structure des Coûts Réels, Fiscalité 2026 & Marges Unitaires

### A. Coûts fixes au lancement : **0,00 € / mois**
| Poste | Solution retenue à 0 € | Limite du palier gratuit | Quand paiera-t-on ? |
| :--- | :--- | :--- | :--- |
| **Structure juridique** | Micro-entreprise (Guichet Unique INPI `formalites.entreprises.gouv.fr`) | 0 € d'immatriculation ; franchise en base de TVA (art. 293 B CGI) jusqu'à 37 500 € CA services | Uniquement au franchissement des seuils légaux |
| **CFE (Impôt local)** | Exonération totale la 1re année civile (art. 1478 CGI) et si CA ≤ 5 000 € | 0 € en année 1 | Année 2 uniquement si CA > 5 000 € (~80 à 250 €/an provisionnés sur ventes) |
| **Compte bancaire** | Compte courant dédié gratuit (Indy 0 €, BoursoBank, Fortuneo) | 0 €/mois | Jamais obligatoire en offre pro payante |
| **Hébergement Web & Base de données** | PaaS gratuit (Vercel / Render / Cloudflare / Fly.io + PostgreSQL Neon/Supabase ou SQLite) | Largement suffisant pour les 500 premiers marchands | Uniquement si trafic > quotas gratuits (financé par CA acquis) |
| **E-mails transactionnels** | Brevo Gratuit (300 e-mails/jour, acteur français conforme RGPD) ou Resend Gratuit (3 000/mois) | ~9 000 accusés/mois gratuits | Au-delà de ~300 boutiques actives simultanées |
| **Acquisition & Prospection** | Scanner interne + Annuaire des Entreprises (`api.gouv.fr`) + SEO + LinkedIn/Email manuel | 0 € | Aucun achat publicitaire |

### B. Coûts variables uniquement sur vente encaissée
1. **Frais de transaction Stripe France (tarif public 2026 vérifié, sans abonnement) :**
   - Cartes européennes (Visa / Mastercard / CB) via Stripe Checkout / Payment Links : **1,5 % + 0,25 €** par transaction réussie.
   - Surcoût Stripe Billing uniquement sur l'option d'abonnement mensuel « Vigie » : **+0,5 %** (soit 2,0 % + 0,25 €).
2. **Cotisations sociales Micro-Entreprise 2026 (Prestations de services commerciales BIC — édition/fourniture d'outil en ligne) :**
   - Taux normal URSSAF 2026 : **21,2 %** + **0,2 %** CFP = **21,4 %** du CA encaissé.
   - *(Variante avec ACRE pour création post-1er juillet 2026 : réduction de 25 %, soit **15,9 %** + **0,2 %** CFP = **16,1 %** la 1re année — par prudence financière, nos calculs de référence retiennent le **taux plein de 21,4 %**).*

### C. Marges réelles par commande (en franchise de TVA, art. 293 B CGI)

| Offre | Prix encaissé | Frais Stripe (`1,5% + 0,25€`) | Coût infra marginal | **Marge brute après paiement** | Cotisations URSSAF + CFP (`21,4%`) | **Revenu Net (avant IR)** | **% Net / CA** |
| :--- | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| **Pack Autonome** | **59,00 €** | 1,14 € | 0,00 € | **57,86 € (98,1 %)** | 12,63 € | **45,23 €** | **76,7 %** |
| **Pack Clé-en-Main 48h** | **129,00 €** | 2,19 € | 0,00 € | **126,81 € (98,3 %)** | 27,61 € | **99,20 €** | **76,9 %** |
| **Pack Agence (5 sites)** | **199,00 €** | 3,24 € | 0,00 € | **195,76 € (98,4 %)** | 42,59 € | **153,17 €** | **77,0 %** |
| **Option Vigie (mensuel)** | **9,00 €/m** | 0,43 € *(2% + 0,25€)* | 0,00 € | **8,57 € (95,2 %)** | 1,93 € | **6,64 €/m** | **73,8 %** |

---

## 5. Parcours d'Achat Client (Sans Friction)

```text
[1. Découverte] Email personnalisé avec capture d'audit / Recherche Google ("bouton rétractation shopify")
       │
       ▼
[2. Preuve Gratuite 15s] Le marchand teste l'URL de sa boutique sur notre Scanner Public (sans e-mail requis)
       │  → Résultat immédiat : ❌ Lien "Renoncer au contrat ici" absent | ❌ Lien RLL mort détecté
       │  → Alerte factuelle : "Vos clients disposent actuellement de 12 mois + 14 jours pour se rétracter"
       ▼
[3. Choix de l'Offre] Comparaison limpide sur la même page :
       ├─ Option A : Je l'installe moi-même en 5 min → 59 € paiement unique
       └─ Option B : Vous l'installez et testez tout pour moi sous 48h → 129 € paiement unique
       │
       ▼
[4. Paiement Réel] Stripe Checkout sécurisé (CB / Apple Pay / Google Pay) + Facture conforme générée
       │
       ▼
[5. Livraison & Activation]
       ├─ Offre 59 € : Accès immédiat au configurateur → URL /r/ma-boutique + snippet JS + guide CMS illustré
       └─ Offre 129 € : Formulaire court d'intégration + livraison sous 48h du Dossier de Preuve Vérifié
       │
       ▼
[6. Vérification Finale] Le marchand relance le Scanner Public → Score 100 % Conforme ✅
```

---

## 6. Ventes Additionnelles (Upsells) & Réachat

1. **Order Bump au checkout (+29 € paiement unique) — Module « Résiliation d'Abonnement en 3 Clics » (art. L.215-1-1) :** Pour les boutiques proposant des box mensuelles, livraisons récurrentes (« Subscribe & Save » Shopify) ou adhésions, ajout d'un second flux distinct intitulé `« Résilier votre contrat »`.
2. **Upgrade vers Clé-en-Main (+70 €) :** Un acheteur de l'offre 59 € qui ne souhaite finalement pas toucher à ses menus Shopify/PrestaShop peut cliquer en 1 clic dans son tableau de bord pour demander notre intervention sous 48h pour la différence (70 €).
3. **Option Récurrente « Vigie Continue » (9 €/mois ou 79 €/an) :** Proposée *après* l'installation réussie (jamais imposée à l'achat) : chaque semaine, notre robot vérifie que la mise à jour d'un thème Shopify ou d'un plugin WordPress n'a pas effacé le lien `« Renoncer au contrat ici »` du pied de page, et alerte le marchand par e-mail en cas de régression.
4. **Réachat multi-boutiques :** Les e-commerçants en série et freelances rachètent des licences unitaires avec -25 % fidélité (44 €) ou basculent sur le Pack Agence 5 boutiques (199 €).
