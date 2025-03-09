# Symfony + Tailwind CSS

Ce projet est une configuration de base de **Symfony 7.2.4** avec **Tailwind CSS 3.4.17**, utilisant **AssetMapper** pour la gestion des assets.

## 📌 Prérequis
Avant de commencer, assurez-vous d'avoir installé les éléments suivants :

- **PHP** >= 8.2  
- **Composer**  
- **Symfony CLI**  
- **Node.js et npm**  
- **Git**  

---

## 🚀 Installation

### 1️⃣ Cloner le projet
```sh
git clone git@github.com:AubourgA/Symfony-tailwind.git
cd Symfony-tailwind
```

### 2️⃣ Installer les dépendances PHP
```sh
composer install
```

### 3️⃣ Configurer la base de données
Créer un fichier `.env.local` pour y renseigner vos paramètres de base de données :

```sh
DATABASE_URL="mysql://db_user:db_password@127.0.0.1:3306/db_name?serverVersion=8.0"
```

### 4️⃣ Lancer le serveur Symfony et Tailwind CSS

```sh
symfony serve
```

Dans un second terminal, lancez la compilation des styles Tailwind en mode watch :

```sh
php bin/console tailwind:build --watch
```

Votre projet Symfony est maintenant accessible sur http://127.0.0.1:8000.