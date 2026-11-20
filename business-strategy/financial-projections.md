# Projections Financières sur 6 et 12 Mois — `RétractaPro`

> **Règles de construction :**
> - **Budget initial à J0 = 0,00 €.** Aucune dépense n'est engagée avant l'encaissement des premières ventes réelles (même l'achat d'un nom de domaine `.fr` à 12 €/an est autofinancé après les premières transactions).
> - ** Régime fiscal & social de référence (France 2026) :** Micro-entreprise en franchise en base de TVA (art. 293 B CGI, donc CA HT = CA TTC encaissé jusqu'à 37 500 € de prestations de services), catégorie **Prestations de services commerciales (BIC)** au **taux plein URSSAF 2026 de 21,2 % + 0,2 % CFP = 21,4 %** (sans même compter le bonus ACRE à 16,1 % qui améliorerait encore le net de +5,3 points). Exonération légale totale de CFE la 1re année civile (art. 1478 CGI).
> - **Frais de transaction réels Stripe France 2026 :** `1,5 % + 0,25 €` par commande carte européenne + `1,5 %` sur l'order bump simultané (+29 €), et `2,0 % + 0,25 €` (incluant +0,5 % Stripe Billing) sur l'abonnement mensuel Vigie à 9 €/mois.

---

## 1. Rappel des Prix et Marges Unitaires

| Offre / Ligne de revenu | Prix unitaire | Frais Stripe | Coût direct | Cotisations URSSAF (`21,4%`) | **Revenu Net (avant IR)** |
| :--- | :---: | :---: | :---: | :---: | :---: |
| **Pack Autonome (`59 €`)** | 59,00 € | 1,14 € | 0,00 € | 12,63 € | **45,23 €** |
| **Pack Clé-en-Main 48h (`129 €`)** | 129,00 € | 2,19 € | 0,00 € | 27,61 € | **99,20 €** |
| **Pack Agence 5 sites (`199 €`)** | 199,00 € | 3,24 € | 0,00 € | 42,59 € | **153,17 €** |
| **Order Bump Résiliation 3 clics (`+29 €`)** | 29,00 € | 0,44 € | 0,00 € | 6,21 € | **22,35 €** |
| **Option Vigie Continue (`9 €/mois`)** | 9,00 € | 0,43 € | 0,00 € | 1,93 € | **6,64 €** |

**Seuil de rentabilité (Point mort) :** **1re vente (Jour 1 commercial)**, car les charges fixes obligatoires au démarrage sont de **0,00 €**.

---

## 2. Scénario 1 — PRUDENT (Démarrage lent, conversion conservatrice)

*Hypothèses :* Démarrage modeste avec 3 commandes le Mois 1 (dont 2 en Clé-en-Main 129 € via prospection directe), progression lente jusqu'à 15 commandes/mois au Mois 6 (~1 vente tous les 2 jours ouvrés) et 10 abonnés à l'option Vigie. Autofinancement du domaine `.fr` (12 €) au Mois 2.

| Mois | Cmds Principales *(59€ / 129€ / 199€)* | Bumps `+29€` & Abonnés `9€/m` | **Chiffre d'Affaires (CA)** | **Frais Stripe** | **Coûts Infra / Outils** | **Cotisations URSSAF (`21,4%`)** | **Revenu Net (avant IR)** |
| :--- | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| **Mois 1** | **3** *(1 / 2 / 0)* | 0 bump · 0 abo | **317,00 €** | 5,50 € | 0,00 € | 67,84 € | **243,66 €** |
| **Mois 2** | **5** *(3 / 2 / 0)* | 1 bump · 1 abo | **473,00 €** | 8,64 € | 12,00 € *(domaine .fr)* | 101,22 € | **351,14 €** |
| **Mois 3** | **8** *(5 / 2 / 1)* | 1 bump · 3 abos | **808,00 €** | 15,00 € | 0,00 € | 172,91 € | **620,09 €** |
| **Mois 4** | **11** *(7 / 3 / 1)* | 2 bumps · 5 abos | **1 102,00 €** | 20,75 € | 0,00 € | 235,83 € | **845,42 €** |
| **Mois 5** | **13** *(9 / 3 / 1)* | 2 bumps · 7 abos | **1 238,00 €** | 23,88 € | 0,00 € | 264,93 € | **949,19 €** |
| **Mois 6** | **15** *(11 / 3 / 1)* | 3 bumps · 10 abos | **1 412,00 €** | 27,88 € | 0,00 € | 302,17 € | **1 081,95 €** |
| **TOTAL 6 MOIS** | **55 commandes** | **9 bumps · 10 abos actifs** | **5 350,00 €** | **101,65 €** | **12,00 €** | **1 144,90 €** | **4 091,45 €** |

- **Projection Année 1 complète (Scénario Prudent — M1 à M12) :** ~150 commandes cumulées, **~14 500 € de CA**, **~11 100 € de Revenu Net** (avec 0 € de risque financier initial).

---

## 3. Scénario 2 — RÉALISTE (Exécution quotidienne régulière → Ventes quotidiennes atteintes en M4)

*Hypothèses :* Exécution disciplinée des 25 diagnostics personnalisés/jour + mise en ligne des 8 guides SEO + recrutement de 1 à 4 agences partenaires/mois. Le cap symbolique d'**1 commande par jour (31 commandes/mois)** est franchi au **Mois 4**, pour atteindre **46 commandes + 35 abonnés Vigie au Mois 6**. Passage optionnel à un petit forfait e-mail transactionnel (15 €/mois) à partir de M5 financé par les revenus.

| Mois | Cmds Principales *(59€ / 129€ / 199€)* | Bumps `+29€` & Abonnés `9€/m` | **Chiffre d'Affaires (CA)** | **Frais Stripe** | **Coûts Infra / Outils** | **Cotisations URSSAF (`21,4%`)** | **Revenu Net (avant IR)** |
| :--- | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| **Mois 1** | **8** *(4 / 4 / 0)* | 1 bump · 2 abos | **799,00 €** | 14,57 € | 0,00 € | 170,99 € | **613,44 €** |
| **Mois 2** | **16** *(10 / 5 / 1)* | 3 bumps · 6 abos | **1 575,00 €** | 29,39 € | 12,00 € *(domaine .fr)* | 337,05 € | **1 196,56 €** |
| **Mois 3** | **24** *(16 / 6 / 2)* | 4 bumps · 12 abos | **2 340,00 €** | 44,64 € | 0,00 € | 500,76 € | **1 794,60 €** |
| **Mois 4** | **31** *(22 / 7 / 2)* | 6 bumps · 18 abos | **2 935,00 €** | 57,09 € | 0,00 € | 628,09 € | **2 249,82 €** |
| **Mois 5** | **39** *(28 / 8 / 3)* | 8 bumps · 26 abos | **3 747,00 €** | 73,62 € | 15,00 € *(quota email)* | 801,86 € | **2 856,52 €** |
| **Mois 6** | **46** *(34 / 8 / 4)* | 10 bumps · 35 abos | **4 439,00 €** | 88,41 € | 15,00 € *(quota email)* | 949,95 € | **3 385,64 €** |
| **TOTAL 6 MOIS** | **164 commandes** | **32 bumps · 35 abos actifs** | **15 835,00 €** | **307,72 €** | **42,00 €** | **3 388,70 €** | **12 096,58 €** |

- **Projection Année 1 complète (Scénario Réaliste — M1 à M12) :** ~460 commandes cumulées + ~85 abonnés Vigie récurrents (765 €/mois de MRR), **~44 200 € de CA** *(attention : point de vigilance à 37 500 € pour anticiper le passage à la TVA collectée sur les clients B2B, neutre pour les sociétés assujetties qui récupèrent la TVA)*, **~33 700 € de Revenu Net avant IR**.

---

## 4. Scénario 3 — AMBITIEUX (Traction forte SEO + Effet réseau Agences Shopify/PrestaShop)

*Hypothèses :* Nos études publiques sur la conformité e-commerce 2026 deviennent une référence partagée dans les communautés Shopify/PrestaShop françaises ; le Scanner gratuit se positionne dans le Top 3 Google sur les requêtes clés dès M2–M3 ; une vingtaine de freelances et agences achètent des Packs 5 boutiques de manière répétée. Atteinte de **~3 ventes/jour en M6**.

| Mois | Cmds Principales *(59€ / 129€ / 199€)* | Bumps `+29€` & Abonnés `9€/m` | **Chiffre d'Affaires (CA)** | **Frais Stripe** | **Coûts Infra / Outils** | **Cotisations URSSAF (`21,4%`)** | **Revenu Net (avant IR)** |
| :--- | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| **Mois 1** | **15** *(9 / 5 / 1)* | 3 bumps · 4 abos | **1 498,00 €** | 27,40 € | 12,00 € *(domaine .fr)* | 320,57 € | **1 138,03 €** |
| **Mois 2** | **28** *(18 / 8 / 2)* | 5 bumps · 12 abos | **2 745,00 €** | 51,72 € | 0,00 € | 587,43 € | **2 105,85 €** |
| **Mois 3** | **44** *(30 / 10 / 4)* | 9 bumps · 25 abos | **4 342,00 €** | 83,50 € | 15,00 € | 929,19 € | **3 314,31 €** |
| **Mois 4** | **62** *(45 / 12 / 5)* | 14 bumps · 42 abos | **5 982,00 €** | 117,62 € | 15,00 € | 1 280,15 € | **4 569,23 €** |
| **Mois 5** | **81** *(60 / 14 / 7)* | 18 bumps · 60 abos | **7 801,00 €** | 154,97 € | 25,00 € *(infra + email)* | 1 669,41 € | **5 951,62 €** |
| **Mois 6** | **99** *(75 / 15 / 9)* | 22 bumps · 85 abos | **9 554,00 €** | 193,13 € | 25,00 € *(infra + email)* | 2 044,56 € | **7 291,31 €** |
| **TOTAL 6 MOIS** | **329 commandes** | **71 bumps · 85 abos actifs** | **31 922,00 €** | **628,34 €** | **92,00 €** | **6 831,31 €** | **24 370,35 €** |

- **Note fiscale importante sur le Scénario Ambitieux (M7–M12) :** Au-delà de **37 500 €** de CA prestations de services encaissés sur l'année (seuil majoré à 41 250 €), l'entreprise sort de la franchise en base de TVA : nous passons alors nos prix en **59 € HT / 129 € HT / 199 € HT** (+20 % TVA récupérable pour 95 % de nos clients professionnels B2B), et le plafond micro-entreprise services étant de **83 600 € HT**, le statut micro reste valable toute l'Année 1 avant éventuel passage en SAS/EURL en Année 2.

---

## 5. Synthèse Comparative des 3 Scénarios à 6 Mois

| Indicateur (Cumul M1 à M6) | Scénario Prudent | Scénario Réaliste | Scénario Ambitieux |
| :--- | :---: | :---: | :---: |
| **Investissement initial requis (J0)** | **0,00 €** | **0,00 €** | **0,00 €** |
| **Coût d'Acquisition Client (CAC pub)** | **0,00 €** | **0,00 €** | **0,00 €** |
| **Nombre de commandes principales** | 55 | 164 | 329 |
| **Chiffre d'affaires brut encaissé** | 5 350,00 € | 15 835,00 € | 31 922,00 € |
| **Frais de transaction Stripe** | 101,65 € *(1,90 %)* | 307,72 € *(1,94 %)* | 628,34 € *(1,97 %)* |
| **Coûts techniques autofinancés** | 12,00 € | 42,00 € | 92,00 € |
| **Cotisations sociales URSSAF (`21,4%`)** | 1 144,90 € | 3 388,70 € | 6 831,31 € |
| **Revenu Net généré (avant IR)** | **4 091,45 €** | **12 096,58 €** | **24 370,35 €** |
| *(Avec éligibilité ACRE `-25%` 2026)* | *(4 375,00 €)* | *(12 935,84 €)* | *(26 062,22 €)* |
