# Project Etudiant

## Description
Le projet **Project Etudiant** est une application web développée avec Symfony. Elle est destinée à la gestion des projets des étudiants, permettant de créer, gérer et suivre des projets académiques. L'application inclut des fonctionnalités telles que la gestion des utilisateurs, l'attribution de projets, la création de tâches et le suivi des progrès.

## Prérequis

Avant de commencer, assurez-vous que vous avez les éléments suivants installés sur votre machine :

- [PHP](https://www.php.net/downloads) (version >= 7.4)
- [Composer](https://getcomposer.org/)
- [Symfony](https://symfony.com/download)
- [MySQL](https://www.mysql.com/) ou [MariaDB](https://mariadb.org/)
- [Git](https://git-scm.com/)

## Installation

1. Clonez ce repository sur votre machine locale :
    ```bash
    git clone https://github.com/kevsi/project-etudiant.git
    cd project-etudiant
    ```

2. Installez les dépendances avec Composer :
    ```bash
    composer install
    ```

3. Configurez votre base de données :
    - Créez une base de données (si ce n'est pas déjà fait).
    - Modifiez le fichier `.env` pour correspondre à votre configuration de base de données. Exemple :
      ```
      DATABASE_URL="mysql://root:password@127.0.0.1:3306/project_etudiant?serverVersion=5.7"
      ```

4. Exécutez les migrations pour créer les tables dans la base de données :
    ```bash
    php bin/console doctrine:migrations:migrate
    ```

5. Lancez le serveur Symfony local :
    ```bash
    symfony server:start
    ```

    Vous pouvez maintenant accéder à votre application via [http://localhost:8000](http://localhost:8000).

## Fonctionnalités

- **Gestion des utilisateurs** : Création, modification, et suppression d'utilisateurs.
- **Gestion des projets** : Création de projets et assignation à des étudiants.
- **Gestion des tâches** : Ajout et suivi des tâches au sein des projets.
- **Suivi des progrès** : Visualisation de l'état d'avancement des projets.

## Développement

### Lancer le serveur Symfony
Pour démarrer le serveur de développement, utilisez la commande suivante :
```bash
symfony server:start
