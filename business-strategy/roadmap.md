# Feuille de Route Opérationnelle sur 30 Jours — `RétractaPro`

> **Principe :** Ce calendrier est un guide d'exécution agile partagé entre l'Agent 01 (CEO) et l'Agent 02 (CTO). Il est piloté par un seul cap : **réduire au minimum le délai entre aujourd'hui et la première transaction réelle confirmée**.

---

## Vue Synoptique des 30 Jours

| Période | Phase | Objectif Principal | Livrable Clé de Validation |
| :--- | :--- | :--- | :--- |
| **Jours 1 à 3** | **1. Découverte & Décision** | Étudier le marché français, classer 12 opportunités, valider la faisabilité technique 0 € avec l'Agent 02 et verrouiller `RétractaPro`. | Stratégie complète + PRD validé dans `/management/decisions.md`. |
| **Jours 4 à 7** | **2. Offre & Test de Volonté de Payer** | **Présenter l'offre commerciale avant la fin du code complet** : pré-auditer 60 boutiques réelles et proposer l'offre Clé-en-Main 129 € + Scanner V0.5. | Landing + Scanner V0.5 + Lien Stripe prêt + premiers retours/pré-commandes réels. |
| **Jours 8 à 15** | **3. Construction & Lancement MVP** | Développer et déployer le MVP V1.0 Self-Serve (59 € / 129 € / 199 €) + portail démo + 5 premières pages guides SEO. | Produit en ligne fonctionnel de bout en bout, testé sur mobile et invités. |
| **Jours 16 à 20** | **4. Commercialisation Active** | Exécuter la routine quotidienne (25 diagnostics/j + 5 agences/j) pour décrocher les **premières ventes réelles confirmées** et livrer les premiers clients. | **Première(s) transaction(s) réelle(s) confirmée(s)** + 1er témoignage client livré. |
| **Jours 21 à 30** | **5. Optimisation & Répétabilité** | Analyser l'entonnoir réel, corriger les frictions de conversion, intensifier les partenariats agences et le SEO pour tendre vers des ventes quotidiennes. | Hausse du taux de conversion Scan → Achat, MRR Vigie amorcé, processus répétable. |

---

## Détail Jour par Jour et Répartition CEO / CTO

### PHASE 1 — Jours 1 à 3 : Recherche, Sélection & Alignement Cofondateurs
- **Agent 01 (CEO) :**
  - [x] Inspection du repository et structuration de `/business-strategy/` et `/management/`.
  - [x] Étude factuelle du marché français 2026 (FEVAD, décret n° 2026-3 du 5 janvier 2026, EAA/RGAA, DUERP, Factur-X, etc.).
  - [x] Classement de 12 opportunités et sélection argumentée de **`RétractaPro`**.
  - [x] Rédaction du modèle économique, de la tarification, de la stratégie d'acquisition 0 € et du PRD (`product-requirements.md`).
- **Agent 02 (CTO) :**
  - [ ] Revue critique de l'opportunité #1 (`RétractaPro`) et validation de la faisabilité à 0 € dans `/management/decisions.md`.
  - [ ] Définition de l'architecture technique sobre dans `/product/` (stack open-source sans coût d'API).

---

### PHASE 2 — Jours 4 à 7 : Validation Terrain & Offre Pré-Développement (Priorité Absolue n° 3)
*Nous n'attendons pas le Jour 15 pour confronter l'offre au marché !*
- **Agent 01 (CEO) :**
  - [ ] Constituer le premier fichier qualifié de **75 boutiques françaises actives non conformes** (Shopify, PrestaShop, Wix ayant un lien RLL mort `ec.europa.eu/consumers/odr` et aucun lien `Renoncer au contrat ici`).
  - [ ] Valider les textes de vente finaux de la page d'accueil et des e-mails transactionnels (accusé de réception D.221-5).
  - [ ] Contacter une première vague test de **30 dirigeants** avec un diagnostic personnalisé fait main et proposer l'offre **Installation Clé-en-Main 48h à 129 €** payable via Stripe.
  - [ ] Mesurer le taux de réponse réel et noter les objections exactes des marchands.
- **Agent 02 (CTO) :**
  - [ ] Mettre en ligne le **Palier V0.5** : Landing page + Scanner d'URL public en temps réel (avec fallback questionnaire 4 questions si WAF) + Portail de démonstration `/r/demo-boutique` + Checkout Stripe.

---

### PHASE 3 — Jours 8 à 15 : Finalisation du MVP V1.0 Self-Serve
- **Agent 02 (CTO) :**
  - [ ] Développer le parcours consommateur complet en 2 étapes (`Renoncer au contrat ici` → `Confirmer la rétractation`) accessible sans compte client.
  - [ ] Implémenter la génération du **récépissé horodaté sur support durable (empreinte SHA-256)** imprimable/téléchargeable + envoi d'e-mail.
  - [ ] Construire l'espace marchand minimaliste (configurateur boutique, récupération du lien/snippet JS, registre des demandes avec compteur 14 jours et export CSV).
  - [ ] Intégrer les webhooks Stripe (59 € / 129 € / 199 € / bump +29 € / option Vigie 9 €/mois) et le back-office `/admin` de suivi des KPIs réels.
  - [ ] Tester la fiabilité mobile, l'accessibilité clavier/contraste et la sécurité (anti-SSRF sur le scanner, rate-limiting).
- **Agent 01 (CEO) :**
  - [ ] Rédiger et livrer les contenus des **5 premiers guides SEO transactionnels** (Shopify, PrestaShop, Wix/Webflow, suppression lien RLL, modèle accusé D.221-5) et les guides d'installation illustrés pas-à-pas.
  - [ ] Préparer la liste de **50 freelances et micro-agences e-commerce français** pour le canal partenaire B2B2B.

---

### PHASE 4 — Jours 16 à 20 : Mise en Ligne Officielle & Conquête des Premières Ventes Réelles
- **Action conjointe CEO + CTO :**
  - [ ] Vérification finale de bout en bout (commande test complète → création boutique → dépôt d'une rétractation invité → réception récépissé → export CSV).
  - [ ] Bascule des clés Stripe en production (`live`) dès validation du compte marchand du porteur.
- **Agent 01 (CEO) :**
  - [ ] Exécution quotidienne stricte : **25 diagnostics personnalisés B2B / jour** + **5 approches agences / jour**.
  - [ ] Publication de la 1re étude chiffrée sur LinkedIn et dans les communautés e-commerce françaises (*« État de conformité réel de 100 boutiques françaises au bouton du 19 juin 2026 »*).
  - [ ] Accompagnement VIP des tout premiers acheteurs (installation vérifiée en < 24h) pour sécuriser une satisfaction de 10/10 et recueillir les premiers avis authentiques.

---

### PHASE 5 — Jours 21 à 30 : Optimisation des Conversions & Systématisation
- **Analyse hebdomadaire stricte dans `/management/sales-results.md` :**
  - Comparer le taux de conversion des visiteurs provenant de la prospection directe vs SEO vs partenaires.
  - Identifier à quelle étape précise les utilisateurs du Scanner gratuit s'arrêtent avant le paiement.
- **Optimisations commerciales (Agent 01) :**
  - Doubler l'effort sur le segment CMS qui convertit le mieux (hypothèse prioritaire à vérifier : **Shopify France** et **agences PrestaShop**).
  - Publier 3 guides SEO supplémentaires sur les objections réelles entendues en vente.
  - Activer la proposition post-achat de l'option **Vigie Continue (9 €/mois)** auprès des premiers clients équipés.
- **Optimisations produit sous condition commerciale stricte (Agent 02) :**
  - *Règle absolue :* **Aucune nouvelle fonctionnalité n'est codée entre J21 et J30 si elle ne lève pas un blocage d'achat exprimé par au moins 2 prospects réels.**

---

## Critères d'Alerte et Règles d'Adaptation

- **Alerte 1 (J+10) :** Si sur 50 diagnostics personnalisés envoyés, moins de 3 dirigeants cliquent/répondent → le message est trop long ou trop technique : simplifier l'accroche autour du seul angle financier (*« Vos clients de Noël ont 12 mois + 14 jours pour demander un remboursement »*).
- **Alerte 2 (J+20) :** Si > 30 dirigeants utilisent le Scanner gratuit et constatent leurs failles mais 0 n'achète à 59 € → contacter personnellement 5 testeurs pour comprendre le frein (besoin d'être rassuré → mettre en avant la garantie « Installé ou Remboursé 14j » ou proposer un appel flash de 10 min sur l'offre 129 €).
