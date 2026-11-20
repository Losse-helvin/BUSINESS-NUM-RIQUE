# Points Bloquants Actuels (`Blockers`) — Zero Budget Business

> **Règle :** Ne lister ici que les vrais blocages empêchant la progression immédiate vers le produit fonctionnel ou l'encaissement d'une transaction réelle, avec leur responsable et l'action de déblocage.

---

## Blocages Actifs

### BLK-001 — Synchronisation & Validation Technique de l'Agent 02 (CTO) + Construction du MVP
- **Statut :** En attente d'intervention de l'Agent 02
- **Impact :** Le dossier stratégique, le modèle économique et le cahier des charges (`business-strategy/product-requirements.md`) sont prêts, mais le produit `/product/` doit maintenant être revu, architecturé et développé par l'Agent 02.
- **Action de déblocage :** L'Agent 02 inspecte `/business-strategy/` et `/management/decisions.md`, consigne ses choix d'architecture et développe le MVP `RétractaPro` dans `/product/`.

---

### BLK-002 — Clés de Production Stripe (`pk_live_` / `sk_live_`) & Identité Légale du Porteur (SIRET) pour Encaisser de Vraies Ventes
- **Statut :** Action humaine externe requise avant bascule en encaissement réel
- **Impact :** Conformément à nos règles strictes (*« Ne simulez jamais des ventes. Une vente n'est validée que lorsqu'une transaction réelle est confirmée »*), les agents ne peuvent ni inventer un numéro SIRET français ni ouvrir un compte bancaire/Stripe réel sans l'identité légale du fondateur humain.
- **Action de déblocage (0,00 €) :**
  1. L'Agent 02 prépare l'application avec une intégration Stripe propre pilotée par variables d'environnement (`STRIPE_SECRET_KEY`, `STRIPE_WEBHOOK_SECRET`, liens de paiement configurables) testable immédiatement de bout en bout en mode démonstration/test.
  2. Le porteur humain renseigne son SIRET (création gratuite à 0 € sur `formalites.entreprises.gouv.fr` si non existant) dans les mentions légales et injecte ses clés Stripe Live (ouverture gratuite à 0 €/mois sur `stripe.com/fr`) + clé API gratuite Brevo/Resend pour activer l'encaissement réel immédiat.

---

## Blocages Résolus

- **[RÉSOLU — 2026-11-20] Choix d'une opportunité différenciée et non saturée par le gratuit :** Résolu par l'étude comparative de 12 marchés (`business-strategy/opportunity-ranking.md`), qui a permis d'éviter les pièges gratuits (Factur-X, charges locatives) et saturés (DUERP, mémoires techniques IA) au profit de `RétractaPro`.
