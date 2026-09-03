# RelancePro AI — version fonctionnelle

- Design SaaS premium dark/violet conservé.
- CRM et données de démonstration.
- Authentification Supabase Email/Password.
- Synchronisation des prospects avec Supabase lorsque l'utilisateur est connecté.
- Ajout / modification / suppression / changement de statut persistants.
- Recherche de chantiers en mode démo uniquement tant qu'une source autorisée n'est pas branchée.
- Analyse photo en pré-analyse et sauvegarde de l'analyse dans Supabase.
- Brouillon de devis modifiable.
- Relances et PWA.

## Variables Vercel

- `SUPABASE_URL`
- `SUPABASE_ANON_KEY`
- `AI_API_URL` (optionnel)
- `AI_API_KEY` (optionnel, serveur uniquement)

La clé Supabase utilisée côté navigateur doit être la clé publishable/anon, jamais `service_role`.

## Supabase

Exécuter `supabase-schema.sql` dans SQL Editor, puis activer Email/Password dans Authentication.
