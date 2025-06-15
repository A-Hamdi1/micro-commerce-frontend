# Micro-Commerce Frontend

Interface utilisateur moderne pour le système de gestion commerciale, développée avec Angular 16.

## Fonctionnalités

- **Gestion des Clients**
  - Liste des clients
  - Ajout de nouveaux clients
  - Modification des informations clients
  - Détails des clients

- **Gestion des Produits**
  - Catalogue des produits
  - Ajout de nouveaux produits
  - Modification des produits
  - Gestion des stocks

- **Gestion des Factures**
  - Liste des factures
  - Création de nouvelles factures
  - Modification des factures
  - Impression des factures
  - Détails des factures

- **Gestion des Règlements**
  - Liste des règlements
  - Ajout de nouveaux règlements
  - Modification des règlements
  - Suivi des paiements

- **Administration**
  - Tableau de bord
  - Gestion des utilisateurs
  - Configuration système

- **Sécurité**
  - Authentification
  - Autorisation basée sur les rôles
  - Protection des routes

## Technologies Utilisées

- Angular 16.2.12
- TypeScript 5.1.3
- Bootstrap 5.3.6
- Chart.js 4.4.9
- NgBootstrap 15.1.2
- FontAwesome 6.7.2
- RxJS 7.8.0
- Ngx-Toastr 19.0.0

## Structure du Projet

```
src/
├── app/
│   ├── admin/              # Module d'administration
│   ├── client-list/        # Liste des clients
│   ├── client-form/        # Formulaire client
│   ├── product-list/       # Liste des produits
│   ├── product-form/       # Formulaire produit
│   ├── facture-list/       # Liste des factures
│   ├── facture-details/    # Détails des factures
│   ├── add-facture/        # Création de factures
│   ├── modifer-facture/    # Modification de factures
│   ├── print-facture/      # Impression de factures
│   ├── reglement-list/     # Liste des règlements
│   ├── reglement-details/  # Détails des règlements
│   ├── add-reglement/      # Création de règlements
│   ├── modifer-reglements/ # Modification de règlements
│   ├── dashboard/          # Tableau de bord
│   ├── login/             # Authentification
│   ├── register/          # Inscription
│   ├── users/             # Gestion des utilisateurs
│   ├── shared/            # Composants partagés
│   ├── services/          # Services Angular
│   ├── models/            # Interfaces et modèles
│   ├── guards/            # Guards d'authentification
│   ├── interceptors/      # Intercepteurs HTTP
│   ├── pipes/             # Pipes personnalisés
│   ├── modal/             # Composants modaux
│   ├── config/            # Configuration
│   ├── navbar/            # Barre de navigation
│   └── footer/            # Pied de page
├── environments/          # Configuration par environnement
└── assets/               # Ressources statiques
```

## Prérequis

- Node.js (version 16.x ou supérieure)
- npm (version 8.x ou supérieure)
- Angular CLI (version 16.2.4)
- Git

## Installation

1. Cloner le repository :
```bash
git clone https://github.com/A-Hamdi1/micro-commerce-frontend.git
cd micro-commerce-frontend
```

2. Installer les dépendances :
```bash
npm install
```

3. Démarrer le serveur de développement :
```bash
npm start
```

L'application sera accessible à l'adresse : http://localhost:4200

## Configuration

### Proxy
Le fichier `proxy.conf.json` est configuré pour rediriger les requêtes API vers le backend :
```json
{
  "/api": {
    "target": "http://localhost:8080",
    "secure": false
  }
}
```

### Nginx
Le fichier `nginx.conf` est configuré pour le déploiement en production.

## Déploiement

1. Construire l'application :
```bash
npm run build
```

2. Les fichiers de production seront générés dans le dossier `dist/`

3. Déployer le contenu du dossier `dist/` sur votre serveur web

## Docker

Le projet inclut un `Dockerfile` pour le déploiement en conteneur :

```bash
# Construire l'image
docker build -t micro-commerce-frontend .

# Exécuter le conteneur
docker run -p 80:80 micro-commerce-frontend
```

## Tests

- Tests unitaires : `npm test`
- Tests e2e : `npm run e2e`

## Contribution

1. Fork le projet
2. Créer une branche pour votre fonctionnalité
3. Commiter vos changements
4. Pousser vers la branche
5. Créer une Pull Request

## Bonnes Pratiques

- Suivre les conventions de style Angular
- Utiliser les composants réutilisables
- Implémenter la gestion d'erreurs
- Optimiser les performances
- Maintenir la documentation à jour

## Support

Pour toute question ou problème, veuillez créer une issue dans le repository GitHub.
