# A&Z FOOD — version 2.3

Site de commande/livraison A&Z FOOD.

## Fonctionnalités
- Menu basé sur les flyers A&Z FOOD
- Panier et suppléments burger
- Minimum de commande 15 €
- Adresse + téléphone + instructions de livraison
- Commande enregistrée côté serveur
- WhatsApp avec récapitulatif prérempli (07 59 29 89 60)
- Espace administrateur `/admin`
- Paiement espèces maintenant
- Stripe prévu pour être activé plus tard
- SQLite configurable via `DATABASE_PATH`

## Mise en ligne Render
1. Créer un Web Service depuis ce dépôt GitHub.
2. Build command : `npm install`
3. Start command : `npm start`
4. Ajouter les variables `NODE_ENV`, `SESSION_SECRET`, `ADMIN_PASSWORD`, `DATABASE_PATH`.
5. Ajouter un Persistent Disk monté sur `/var/data` si le service utilise SQLite en production.
6. Mettre `BASE_URL` sur l'URL publique du service.

## Important
Ne jamais mettre `.env`, les mots de passe ou les clés Stripe dans GitHub. Utiliser les variables d'environnement de l'hébergeur.
