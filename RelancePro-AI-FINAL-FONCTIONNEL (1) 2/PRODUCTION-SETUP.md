# RelancePro AI — passage en production

## 1. Supabase
Créer un projet puis exécuter `supabase-schema.sql`.
Activer Email/Password dans Authentication.
Renseigner dans `config.js` :
- SUPABASE_URL
- SUPABASE_ANON_KEY

Ne jamais mettre de clé `service_role` dans le frontend.

## 2. IA
Créer les variables Vercel :
- AI_API_URL
- AI_API_KEY

Le navigateur appelle `/api/ai`; la clé reste côté serveur.

## 3. Données de chantiers
Brancher uniquement des sources dont l'API/usage autorise la collecte.
Conserver `is_demo=true` pour les données fictives.

## 4. Paiement
Prévoir Stripe Checkout côté serveur et webhooks pour synchroniser le statut d'abonnement.

## 5. Avant mise en vente
Tester :
- création de compte
- isolation des données entre deux comptes
- ajout/modification/suppression prospect
- upload photo
- génération de devis
- relances
- mobile
- erreurs réseau
- suppression de compte/données
