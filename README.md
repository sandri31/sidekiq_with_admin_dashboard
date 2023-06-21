# Projet Rails avec Sidekiq et Devise
![Capture d’écran du 2023-06-21 13-14-16](https://github.com/sandri31/sidekiq_with_admin_dashboard/assets/85675011/cd9741f1-a2ea-4b9c-9481-de2cd0e188fb)

Ce projet est une démonstration d'une application Ruby on Rails intégrant Sidekiq pour le traitement des tâches en arrière-plan et Devise pour l'authentification des utilisateurs.

## Fonctionnalités principales

1. **Authentification des utilisateurs avec Devise** : Le projet utilise Devise pour gérer l'authentification des utilisateurs.

2. **Traitement des tâches en arrière-plan avec Sidekiq** : Le projet utilise Sidekiq pour gérer le traitement des tâches en arrière-plan. 

3. **Contrôle d'accès basé sur les rôles** : Les utilisateurs sont assignés soit le rôle d'administrateur, soit le rôle d'utilisateur standard. Seuls les administrateurs ont accès au tableau de bord Sidekiq.

## Comment ça marche

Lorsqu'un utilisateur navigue sur le site, il peut se connecter via Devise. S'il est un administrateur, il a accès à une interface d'administration où il peut surveiller les tâches Sidekiq en cours d'exécution grâce à un dashboard (voir screen ci-dessus). Les tâches Sidekiq sont utilisées pour exécuter des opérations en arrière-plan, comme envoyer des courriels ou effectuer des calculs intensifs.

## Technologies utilisées

- Ruby on Rails 7
- Sidekiq
- Devise
- PostgreSQL (pour la base de données)

## Licence

Ce projet est sous licence MIT. Voir le fichier LICENSE pour plus de détails.
