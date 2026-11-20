# Étude de Marché — France (Novembre 2026)

> **Règle de rigueur :** Aucune statistique inventée. Toutes les données réglementaires, tarifaires et sectorielles ci-dessous proviennent de sources publiques françaises vérifiables en 2026 (FEVAD, Légifrance, Code de la consommation, Code du travail, DGCCRF, Altares, CAPEB, Arcom) et de relevés directs des offres concurrentes actives sur le marché français.

---

## 1. Méthodologie de Recherche

Pour identifier une opportunité capable de générer une **première vente rapide puis des ventes quotidiennes avec 0 € de budget initial**, nous avons filtré le marché français selon 5 critères impératifs :
1. **Douleur financière ou légale mesurable :** Le problème doit coûter de l'argent réel (perte de chiffre d'affaires, remboursements forcés, amendes administratives actives, perte d'heures facturables).
2. **Urgence réglementaire ou opérationnelle en 2026 :** Existence d'un déclencheur concret poussant le client à agir *cette semaine* et non « un jour ».
3. **Absence d'alternative gratuite clé-en-main :** Si des outils gratuits sans inscription couvrent déjà 100 % du besoin, la volonté de payer à l'unité s'effondre.
4. **Cibles repérables publiquement à 0 € :** Possibilité d'identifier et de qualifier des prospects précis sans acheter de bases de données ni de publicité.
5. **Faisabilité technique déterministe à 0 € :** Aucun abonnement serveur initial, aucun coût d'API d'intelligence artificielle par requête requis au lancement, respect strict du périmètre légal (notamment l'article 54 de la loi du 31 décembre 1971 encadrant le conseil juridique).

---

## 2. Analyse des 6 Pôles de Problèmes Étudiés en France

### Pôle A — Conformité E-Commerce & Vente en Ligne B2C ( Choc réglementaire du 19 juin 2026 )
- **Taille du marché vérifiée :** Selon le bilan annuel **FEVAD 2026** (portant sur l'exercice 2025 et le S1 2026), la France compte **158 200 sites marchands actifs** (+7 % sur un an) générant **196,4 milliards d'euros** de chiffre d'affaires et **3,2 milliards de transactions** auprès de **42,2 millions de cyberacheteurs**. Près de **69 % des sites réalisent moins de 100 000 € de CA annuel** (des TPE, DNVB, commerçants et solopreneurs sans équipe juridique ni développeur interne), avec un panier moyen de **59,70 €** au T2 2026. À cela s'ajoutent des milliers d'organismes de formation en ligne, coachs, éditeurs de box et SaaS B2C.
- **Le fait générateur majeur :** Depuis le **19 juin 2026**, l'**ordonnance n° 2026-2** et le **décret n° 2026-3 du 5 janvier 2026** (transposant la directive UE 2023/2673 et l'étendant en France à *tous* les contrats conclus à distance en ligne avec des consommateurs via les articles **L.221-21** et **D.221-5** du Code de la consommation) imposent un **bouton de rétractation en ligne obligatoire** :
  - Libellé d'entrée imposé : **« renoncer au contrat ici »** (ou formule analogue dénuée d'ambiguïté — les mentions « Retours », « SAV » ou « Contact » sont non conformes).
  - Accessibilité directe, visible et permanente pendant tout le délai de 14 jours, **sans obliger le client à se connecter à un compte** (gestion obligatoire des commandes invités).
  - Parcours en **2 étapes** : formulaire d'identification (nom, contrat/commande, moyen électronique de réponse) suivi d'un bouton de validation intitulé **« confirmer la rétractation »**.
  - Envoi dans un délai raisonnable d'un **accusé de réception horodaté sur support durable** (date, heure, contenu de la déclaration) et mise à jour de l'information précontractuelle (art. L.221-5, 7°).
- **Double sanction financière :**
  1. **Prolongation automatique du délai de rétractation à 12 mois + 14 jours** de plein droit en cas de manquement à l'information ou au dispositif.
  2. **Amende administrative DGCCRF** jusqu'à **15 000 €** (personne physique) et **75 000 €** (personne morale, art. L.242-13), doublée en récidive.
- **Infractions connexes massives constatées sur les sites français fin 2026 :**
  - **Lien mort RLL/ODR :** La plateforme européenne de règlement en ligne des litiges (`ec.europa.eu/consumers/odr`) est **définitivement fermée depuis le 20 juillet 2025** (Règlement UE 2024/3228). Une grande partie des boutiques françaises affichent encore ce lien périmé dans leurs CGV.
  - **Médiateur de la consommation :** Obligatoire pour tout vendeur B2C (art. L.616-1, amende 3 000 € PP / 15 000 € PM). Selon le bilan décennal publié par la DGCCRF en 2025, **près de 10 000 professionnels ont été contrôlés en une seule année** sur ce point.
  - **Résiliation en 3 clics :** Obligatoire pour tout contrat à abonnement souscrit en ligne (art. L.215-1-1, amende 15 000 € / 75 000 €).
- **Défaillance des solutions existantes :**
  - **Shopify** ne fournit pas nativement le parcours français en 2 étapes « Renoncer au contrat ici » → « Confirmer la rétractation » sans compte.
  - **PrestaShop**, **Wix**, **Webflow**, **Squarespace** et **Systeme.io** n'intègrent aucune fonction native couvrant le décret n° 2026-3.
  - **WooCommerce** a introduit une base technique désactivée par défaut et non reliée au pied de page, ou dépend de plugins tiers isolés.

### Pôle B — Accessibilité Numérique PME (European Accessibility Act / RGAA)
- **Cadre et sanctions :** Depuis le **28 juin 2025** (directive EAA 2019/882, loi n° 2023-171), les entreprises privées dépassant **10 salariés OU 2 millions d'euros de CA** proposant un service e-commerce ou numérique B2C doivent respecter l'accessibilité (RGAA 4.1.2 / WCAG) et publier une **déclaration d'accessibilité**, un **schéma pluriannuel sur 3 ans** et un **plan d'action annuel**. En 2026, la DGCCRF et l'Arcom mènent des contrôles avec des amendes jusqu'à **50 000 € par service non conforme** et **25 000 €** pour défaut de déclaration/schéma.
- **Concurrence relevée :** Agences spécialisées entre **2 000 € et 6 000 € HT** l'audit (`Sisméo` forfait accompagné à **1 490 € HT**, `kacz-web` audit dès **2 100 € HT** / pack documents à **790 €**). Mais plusieurs SaaS français occupent déjà l'entrée de gamme automatisée : `DeclareAccess` (**49 €/site**), `ConformCheck` (**29 € à 49 €**), `RGAA-IA` (**190 €** les 4 documents), `RGAA Checker` (**69 €/mois**).
- **Limite critique :** Les micro-entreprises (<10 salariés et <2 M€ CA) sont **exemptées**, ce qui exclut la majorité des petites boutiques indépendantes, et un audit RGAA complet sur 106 critères exige légalement une part de vérification humaine (lecteur d'écran, navigation clavier).

### Pôle C — Obligations RH TPE/PME : DUERP 2026 & Transparence Salariale
1. **DUERP (Document Unique d'Évaluation des Risques Professionnels) :**
   - Obligatoire dès le 1er salarié (art. R.4121-1 Code du travail). Depuis le **27 juin 2026** (loi n° 2026-534 du 25 juin 2026), la DREETS peut prononcer sans juge une **amende administrative jusqu'à 4 000 € par salarié concerné** (8 000 € en récidive).
   - **Réalité concurrentielle relevée :** Marché extrêmement saturé fin 2026 par des générateurs en ligne très bien référencés en achat unique : `DUERP Clair` (**35 €**), `Phrolo` (**39 € HT**), `ConformitéBTP` (**39 € TTC**), `DUERP en direct` (**49 €**), `DUERP TPE` (**49 € TTC**), en plus de l'outil gratuit officiel européen `OiRA` (INRS). Difficile d'y percer rapidement à 0 € de budget pub SEO face à des domaines installés.
2. **Directive Transparence Salariale (UE 2023/970 — échéance juin / fin 2026) :**
   - Interdiction de la mention « salaire selon profil », obligation d'afficher une fourchette salariale sincère dès l'offre d'emploi ou avant entretien, interdiction de demander le salaire passé, droit des salariés d'obtenir sous 2 mois les rémunérations moyennes par sexe pour un travail de valeur égale (dès 1 salarié).
   - **Réalité concurrentielle :** Les grands logiciels (`Figures` dès **2 500 €/an**, `Nibelis` dès **4 500 €/an**, `Foederis` **8 000–15 000 €/an**) visent les ETI. Il existe un vrai trou pour les PME de 10–99 salariés, mais la non-conformité interne d'une grille salariale est plus difficile à prouver de l'extérieur que sur un site e-commerce, exception faite des offres d'emploi publiques affichant encore « selon profil ».

### Pôle D — Artisans & TPE : Devis conformes, Impayés & Marchés Publics
- **Poids administratif et impayés :** Selon le baromètre CAPEB, près d'un artisan du bâtiment sur deux consacre un quart de son temps (plus d'1 jour/semaine) à l'administratif. Selon **Altares (S1 2025)**, le retard moyen de paiement des TPE françaises atteint **15,53 jours** (record européen, sur fond de près de 70 000 défaillances d'entreprises).
- **Mentions obligatoires des devis BTP :** L'oubli de la mention **déchets de chantier** (art. L.541-21-2-3 Code de l'environnement) ou du **médiateur** coûte jusqu'à **3 000 € (EI) / 15 000 € (société)**. Toutefois, les logiciels BTP établis (`Obat`, `Tolteck`, `Costructor`, `Mediabat`) intègrent déjà ces mentions.
- **Mémoires techniques BTP :** Forte demande (consultants à 800–2 500 €), mais concurrence IA très dense en 2026 (`AlveoWeb` dès **29,90 € HT/mémoire**, `Maître AO` **39 €/mois**, `BatiRedac` **69 €/mois**, `ConformitéBTP` **79 €**, `BâtiOffre` **99 €**, `Offralis` **99 €/mois**) et nécessité d'appels LLM lourds sur des PDF CCTP de 100 pages (incompatible avec une contrainte stricte de 0 € d'API au démarrage).

### Pôle E — Réforme de la Facturation Électronique (1er sept. 2026 / 1er sept. 2027)
- **Cadre légal :** Réception obligatoire pour toutes les entreprises depuis le **1er septembre 2026** ; émission obligatoire au format structuré (Factur-X / UBL / CII via Plateforme Agréée) au **1er septembre 2027** pour les TPE, PME et micro-entreprises (amendes prévues par la loi de finances n° 2026-103 : 50 €/facture et 500 € pour absence de PA).
- **Piège commercial identifié grâce à l'étude :** De nombreux générateurs et convertisseurs **Factur-X 100 % gratuits et sans inscription** existent déjà fin 2026 (`factureelectronique.eu`, `facturevalide.fr`, `verif-facturx.fr`, `scanfacture.fr`, `e-facturepro.com` gratuit / 12 €). Vendre un simple générateur Factur-X se heurterait immédiatement à un mur de gratuité.

### Pôle F — Gestion Locative & Litiges Dépôt de Garantie (Immobilier)
- **Régularisation des charges (Bailleurs) :** Nombreux simulateurs conformes au décret n° 87-713 déjà **100 % gratuits** (`baildelocation.com`, `contrat-de-location.com`, `hestia.software`, `faireplace.com`, `macalculatriceenligne.com`). Volonté de payer quasi nulle pour un calculateur isolé.
- **Récupération de dépôt de garantie retenu abusivement (Locataires B2C) :** Problème fréquent (pénalité légale de 10 % du loyer HC par mois de retard, art. 22 loi du 6 juillet 1989 ; des acteurs comme `Dossier Juridique` vendent des dossiers autour de **14,99 €**). Cependant : panier très faible (~15 €), achat unique non récurrent (un locataire déménage tous les 3–4 ans), impossible de cibler un locataire lésé en prospection directe sans publicité Google Ads, et **risque pénal élevé d'exercice illégal du droit** (art. 54 loi du 31 décembre 1971) si l'outil rédige une mise en demeure personnalisée qualifiant juridiquement les faits.

---

## 3. Cartographie Concurrentielle Détaillée du Segment Sélectionné (Bouton de Rétractation 2026)

| Type d'acteur | Exemples relevés en France (fin 2026) | Prix constaté | Limites / Faiblesses exploitables par notre offre |
| :--- | :--- | :--- | :--- |
| **Fonctions natives CMS** | Shopify, PrestaShop, Wix, Webflow, Systeme.io | Inclus dans CMS | **Non conformes seules** au décret n° 2026-3 : pas de parcours 2 étapes « Renoncer au contrat ici » → « Confirmer la rétractation » accessible sans compte avec accusé horodaté. |
| **Plugins isolés WooCommerce** | `retractation-woo`, `Herroepingsknop`, `EasyReturn` | Gratuit (WP uniquement) | Réservés exclusivement à WooCommerce ; certains exigent que le client soit connecté à son compte (illégal pour les commandes invités) ; aucune couverture Shopify / PrestaShop / Wix / SaaS ; aucun scan global du site (lien RLL mort, médiateur). |
| **Modules PrestaShop** | Modules Addons / `Prestaify` | 50 € à 90 € HT | Liés à une version précise de PrestaShop (risque de conflit lors des mises à jour 1.7 / 8 / 9), installation technique requise, pas de couverture multi-CMS. |
| **SaaS en abonnement** | `BackToMe` | **25 € HT/mois** (250–300 € HT/an) | **Forte résistance psychologique à l'abonnement mensuel** chez les 69 % de boutiques françaises réalisant < 100 k€ de CA qui souffrent déjà de « SaaS fatigue ». |
| **Prestation agence sur-mesure** | `WebSentinel` (149 € + 49 €/an), freelances web, avocats | **149 € à 1 500 €+** | Délai d'intervention humain pour chaque boutique, coût élevé chez les agences et cabinets, pas de diagnostic instantané en libre-service. |

---

## 4. Synthèse des Signaux de Demande et Fenêtre de Tir

1. **L'échéance légale est DÉJÀ dépassée (19 juin 2026) :** Nous ne vendons pas une conformité hypothétique pour 2028. Tout site B2C sans bouton « Renoncer au contrat ici » est *actuellement* en infraction et exposé à la prolongation de rétractation de 12 mois + 14 jours sur chaque vente encaissée aujourd'hui.
2. **Saisonnalité maximale (Novembre – Janvier) :** La période Black Friday / Noël concentre le pic annuel des commandes e-commerce en France — et mécaniquement le pic des demandes de rétractation de janvier. Sécuriser le délai à 14 jours (au lieu de 12 mois et 14 jours) avant les ventes de fin d'année a un **ROI immédiat et évident** pour tout marchand.
3. **Vérifiabilité externe à 100 % :** Contrairement à un logiciel interne, l'absence du lien « Renoncer au contrat ici » ou la présence du lien mort `ec.europa.eu/consumers/odr` se constate publiquement en 3 secondes sur n'importe quelle boutique française — ce qui permet une prospection B2B ultra-pertinente à **0 € de coût d'acquisition**.
