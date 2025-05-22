# How to use the starter kit

## Prérequis techniques

- PHP: >= 8.2

## Utiliser le starter kit comme skeleton

- Créer un repo sur le gitHub de SAMs : <a href="https://github.com/ShareAndMove">https://github.com/ShareAndMove</a>

- Cloner le repository
``` bash
git clone lien-du-repo
```

- Créer un projet par composer en utilisant le lien du starter kit comme repositories
``` bash
composer create-project sams/symfony-skeleton . --repository-url=https://github.com/ShareAndMove/Symfony_Starter_Kit.git
```

- Modifier les informations du projet dans le <code>composer.json</code>.
``` JSON
{
  "name": "sams/symfony-skeleton",
  "type": "project",
  "license": "proprietary",
  "description": "Sams Symfony project starter kit",
  "minimum-stability": "stable",
  "prefer-stable": true
}
```

- Pousser votre nouveau projet sur GitHub
``` bash
git push
```

Voilà, votre nouveau projet est en place sur GitHub !

## Let's get started

- Créer le fichier <code>.env.local</code> à partir du fichier <code>.env</code> et remplir les variables d'environnement.

- Installer les dépendances
``` bash
composer install
```

- Créer votre base de donnée locale
``` bash
php bin/console d:d:c
```

- Initier l'instance locale de <code>git flow</code>
``` bash
git flow init
```

- Créer une branche de feature
``` bash
git flow feature start nom-de-la-feature
```

Bien joué, vous pouvez commencer à coder !
