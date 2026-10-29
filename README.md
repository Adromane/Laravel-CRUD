# Laravel CRUD — Gestion des employés

Application web de gestion des employés développée avec **Laravel 10**. Ce projet permet d'effectuer les opérations CRUD (*Create, Read, Update, Delete*) sur les informations des employés.

## Fonctionnalités

- Ajouter un nouvel employé.
- Afficher la liste des employés.
- Modifier les informations d'un employé.
- Supprimer un employé.
- Enregistrer les données dans une base de données avec Eloquent ORM.

## Technologies utilisées

- PHP 8.1+
- Laravel 10
- Blade
- Vite
- JavaScript
- Base de données compatible avec Laravel

## Informations sur les employés

Chaque employé possède les champs suivants :

- **Nom** : nom de l'employé.
- **Date de naissance** : date de naissance.
- **Téléphone** : numéro de téléphone, facultatif.

## Installation

### 1. Cloner le projet

```bash
git clone https://github.com/Adromane/Laravel-CRUD.git
cd Laravel-CRUD
```

### 2. Installer les dépendances PHP

```bash
composer install
```

### 3. Configurer l'environnement

Copiez le fichier `.env.example` :

```powershell
Copy-Item .env.example .env
```

Générez la clé de l'application :

```bash
php artisan key:generate
```

Configurez ensuite la connexion à votre base de données dans `.env`.

### 4. Préparer la base de données

```bash
php artisan migrate
```

### 5. Installer les dépendances front-end

```bash
npm install
```

Pour compiler les ressources :

```bash
npm run build
```

### 6. Lancer l'application

```bash
php artisan serve
```

Ouvrez ensuite l'adresse indiquée dans le terminal, généralement `http://127.0.0.1:8000`.

## Routes principales

| Méthode | Route | Fonction |
|---|---|---|
| GET | `/` | Redirection vers la liste des employés |
| GET | `/employee` | Afficher les employés |
| POST | `/employee` | Ajouter un employé |
| GET | `/employee/{employee}/edit` | Modifier un employé |
| PUT/PATCH | `/employee/{employee}` | Mettre à jour un employé |
| DELETE | `/employee/{employee}` | Supprimer un employé |

## Auteur

**Patrik Adromane Vieira Gomes**

- GitHub : https://github.com/Adromane
- Portfolio : https://patrick97.netlify.app/#/home
- LinkedIn : https://www.linkedin.com/in/patrik-adromane-vieira-gomes-14970722b/

---

Projet réalisé dans le cadre de la pratique du développement web avec Laravel et des opérations CRUD.
