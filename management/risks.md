# Registre des Risques & Plans de Mitigation — Zero Budget Business

> **Principe :** Identifier lucidement tout ce qui peut empêcher la première vente, détruire la marge à 0 € ou créer un risque légal en France, et prévoir une parade gratuite immédiate.

---

## 1. Risques Légaux & Réglementaires (France)

| ID | Risque identifié | Gravité | Probabilité | Mitigation concrète à 0 € |
| :---: | :--- | :---: | :---: | :--- |
| **R-01** | **Requalification en exercice illégal du droit (Art. 54 loi du 31/12/1971)** si nous promettons de « rédiger des CGV sur mesure » ou de « délivrer un audit juridique personnalisé ». | Critique | Faible *(si cadré)* | Positionnement strict : **logiciel technique d'interface et d'horodatage** + détection technique de balises HTML + rappel documentaire des textes publics Légifrance. Mention explicite dans nos CGU et sur le site. |
| **R-02** | **Non-conformité du parcours généré aux articles L.221-21 & D.221-5** (ex. imposer un compte client, imposer un motif, mauvais libellé du bouton). | Élevée | Très faible | Respect strict des règles `RM-01` à `RM-06` du PRD : libellés exacts `« Renoncer au contrat ici »` et `« Confirmer la rétractation »`, accès invité sans mot de passe, motif facultatif, récépissé durable horodaté SHA-256. |
| **R-03** | **Plainte CNIL pour prospection B2B abusive (spam).** | Moyenne | Faible | Prospection exclusivement B2B vers des boutiques actives, volume limité (25 messages vérifiés humainement/jour), constat factuel réel lié à la boutique, lien/mention d'opposition honoré immédiatement. |
| **R-04** | **Confusion avec un service officiel de l'État / DGCCRF.** | Élevée | Nulle | Bannière claire en pied de page : *« RétractaPro est un outil logiciel privé indépendant, non affilié à la DGCCRF ni à l'administration publique »*. |

---

## 2. Risques Commerciaux & Marché

| ID | Risque identifié | Gravité | Probabilité | Mitigation concrète à 0 € |
| :---: | :--- | :---: | :---: | :--- |
| **R-05** | **Inertie du marchand (« je verrai plus tard »).** | Élevée | Moyenne | Mettre en avant non pas seulement l'amende théorique, mais le **coût commercial immédiat** : prolongation automatique du droit de rétractation des clients à **12 mois + 14 jours** sur toutes les commandes en cours (Black Friday / Noël), + offre **Clé-en-Main 129 €** zéro effort. |
| **R-06** | **Déploiement futur d'une fonction native complète par Shopify ou PrestaShop.** | Moyenne | Moyenne *(à 6–12 mois)* | Même plusieurs mois après le 19 juin 2026, Shopify et PrestaShop ne couvrent pas le formalisme français complet sans configuration. D'ici une éventuelle couverture native partielle, nous aurons amorti 0 € d'investissement, constitué une base B2B et pourrons étendre la suite (module Résiliation 3 clics L.215-1-1, Vigie globale pied de page B2C : médiateur, RLL, mentions légales). |
| **R-07** | **Concurrence des plugins gratuits sur WooCommerce.** | Faible | Avérée | Ne pas concentrer la prospection sortante sur les profils techniques WordPress ; cibler prioritairement **Shopify, PrestaShop, Wix, Webflow, Systeme.io** et les **agences web** où la valeur du clé-en-main universel est maximale. |

---

## 3. Risques Techniques & Financiers (À compléter / enrichir par l'Agent 02)

| ID | Risque identifié | Gravité | Probabilité | Mitigation concrète à 0 € |
| :---: | :--- | :---: | :---: | :--- |
| **R-08** | **Blocage du Scanner d'URL par des pare-feux anti-bot (Cloudflare, DataDome) sur certaines boutiques.** | Moyenne | Élevée *(~20–30 % des sites)* | Prévu dans le PRD (`Section 4.4`) : si le fetch reçoit un `403`/timeout, bascule fluide et immédiate vers l'**Auto-Diagnostic Interactif en 4 clics (30s)** pour ne perdre aucun prospect. |
| **R-09** | **Dépassement des quotas gratuits d'envoi d'e-mails (ex. 300/jour Brevo) si une grosse boutique s'inscrit.** | Moyenne | Faible au début | Plafonner contractuellement la licence unique 59 € à **50 rétractations/mois** (couvre >95 % des TPE) ; au-delà, bascule sur le plan Haut Volume à **19 €/mois** qui finance largement un forfait SMTP dédié. De plus, le récépissé durable est **immédiatement téléchargeable à l'écran** par le consommateur même en cas de latence e-mail. |
| **R-10** | **Faille SSRF via le champ URL du Scanner public.** | Critique | Faible *(si filtré)* | Filtrage strict côté serveur par l'Agent 02 : interdiction des IP locales/privées/métadonnées cloud, résolution DNS vérifiée, schémas `http/https` uniquement, timeout strict. |
| **R-11** | **Rétention temporaire de fonds KYC par Stripe lors des premières ventes.** | Faible | Moyenne | Compléter intégralement le profil KYC Stripe (identité, SIRET micro-entreprise, descriptif clair du logiciel SaaS B2B et conditions de remboursement visibles sur le site avant le 1er encaissement). Comme nos coûts fixes sont à 0 €, un délai de virement initial de 7 jours ne met jamais l'entreprise en danger. |
