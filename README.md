# projet-3

Base de données : MySQL 8

Structure :
── db/
│   ├── schema.sql             # Schéma MySQL + données démo
│   └── init.js

Configurer la base de données

Créez un fichier `.env` à partir de `.env.example` :
```bash
cp .env.example .env
```
Éditez `.env` avec vos identifiants MySQL :
```env
PORT=3000
DB_HOST=localhost
DB_PORT=3306
DB_USER=root
DB_PASSWORD=mon_mot_de_passe
DB_NAME=nom_de_la_base_de_donnée
JWT_SECRET=changez_cette_cle_secrete
```
Initialiser la base de données

Assurez-vous que le serveur MySQL est lancé, puis :
```bash
npm run init-db
```
Cette commande :
crée la base `afrovibe`
crée toutes les tables
insère les catégories par défaut
crée trois comptes de démonstration
 Lancer le serveur
```bash
npm start
```
Ouvrez votre navigateur sur : http://localhost:3000
👤 Comptes de démonstration

Email	Mot de passe	Rôle
`admin@afrovibe.com`	`password123`	Administrateur
`awa@afrovibe.com`	`password123`	Organisateur
`moussa@afrovibe.com`	`password123`	Participant
