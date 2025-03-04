# Edicom Backend

![image](https://github.com/user-attachments/assets/b72f9b66-c71c-4bd1-8487-16315b7c7995)


## Description
**Edicom Backend** est une API REST développée avec **Symfony 5.4.48**. Elle fournit des fonctionnalités essentielles pour gérer les utilisateurs et l'authentification. L'API est documentée avec **Swagger** et inclut des tests unitaires pour garantir sa robustesse.

## Auteur
👤 **Yassine Elmiri**  
🔗 [GitHub Repository](https://github.com/yassineelmiri/Edicom_backend)

---

## 🛠 Technologies utilisées
- **Symfony 5.4.48** - Framework PHP
- **Swagger (NelmioApiDoc)** - Documentation de l'API
- **PHPUnit** - Tests unitaires
- **Doctrine ORM** - Gestion de la base de données
- **MySQL** - Base de données

---

## 🚀 Installation

### Prérequis
- **PHP >= 7.4**
- **Composer**
- **Symfony CLI**
- **MySQL**

### Étapes d'installation

1. **Cloner le projet**
   ```bash
   git clone https://github.com/yassineelmiri/Edicom_backend.git
   cd Edicom_backend
   ```

2. **Installer les dépendances**
   ```bash
   composer install
   ```

3. **Configurer l'environnement**
   Copier le fichier `.env` et modifier les variables nécessaires :
   ```bash
   cp .env .env.local
   ```
   Modifier la connexion à la base de données dans `.env.local` :
   ```ini
   DATABASE_URL="mysql://root:password@127.0.0.1:3306/edicom_db"
   ```

4. **Créer la base de données**
   ```bash
   php bin/console doctrine:database:create
   php bin/console doctrine:migrations:migrate
   ```

5. **Démarrer le serveur Symfony**
   ```bash
   symfony server:start
   ```

---

## 📌 Documentation API
L'API est documentée avec Swagger. Pour accéder à la documentation interactive :
```bash
http://127.0.0.1:8000/api/doc
```

---

## ✅ Tests Unitaires
Pour exécuter les tests PHPUnit :
```bash
php bin/phpunit
```

---

## 📂 Structure du projet
```
Edicom_backend/
│── config/                 # Configuration du projet
│── migrations/             # Fichiers de migration de la base de données
│── src/
│   ├── Controller/         # Contrôleurs Symfony
│   ├── Entity/             # Entités Doctrine
│   ├── Repository/         # Repositories pour les requêtes SQL
│   ├── Security/           # Gestion de l'authentification
│   ├── Kernel.php          # Noyau de l'application Symfony
│── tests/                  # Tests unitaires
│── .env                    # Variables d'environnement
│── composer.json           # Dépendances PHP
│── README.md               # Documentation du projet
```
