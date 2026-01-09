# GSCO - Système de Gestion Scolaire

![Laravel](https://img.shields.io/badge/Laravel-FF2D20?style=for-the-badge&logo=laravel&logoColor=white)
![PHP](https://img.shields.io/badge/PHP-777BB4?style=for-the-badge&logo=php&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-005C84?style=for-the-badge&logo=mysql&logoColor=white)

## 📋 Description
Application web de gestion scolaire complète développée avec Laravel 9. Système modulaire pour la gestion des étudiants, professeurs, notes, absences et emplois du temps.

## ✨ Fonctionnalités principales
- 👥 **Gestion des utilisateurs** (Admin, Professeurs, Étudiants, Parents)
- 🏫 **Gestion des classes et matières**
- 📊 **Saisie et consultation des notes**
- 📅 **Gestion des absences et retards**
- 🕐 **Emplois du temps dynamiques**
- 📈 **Tableaux de bord statistiques**
- 📄 **Génération de bulletins (PDF)**
- 🔐 **Système d'authentification sécurisé**

## 🛠️ Stack technique
- **Backend** : Laravel 9, PHP 8.5
- **Frontend** : Blade, Bootstrap 5, JavaScript
- **Base de données** : MySQL
- **Outils** : Composer, Git, GitHub
- **Serveur** : Apache (WAMP)

## 🚀 Installation

### Prérequis
- PHP >= 8.1
- Composer
- MySQL 5.7+
- Git

### Étapes d'installation
```bash
# 1. Cloner le projet
git clone https://github.com/humilite/GSCO.git
cd GSCO

# 2. Installer les dépendances PHP
composer install

# 3. Configurer l'environnement
cp .env.example .env
php artisan key:generate

# 4. Configurer la base de données dans .env
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=gestion_scolaire
DB_USERNAME=root
DB_PASSWORD=

# 5. Créer la base de données et lancer les migrations
php artisan migrate --seed

# 6. Lancer le serveur de développement
php artisan serve

# 7. Accéder à l'application
# http://localhost:8000