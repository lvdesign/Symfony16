

## Télécharger les vendors
Avec Composer bien évidemment :

    php composer.phar install

## Créez la base de données
Si la base de données symfony existe pas :

    php bin/console doctrine:database:create

Ajoutez les fixtures :

    php bin/console doctrine:fixtures:load

Publiez les assets dans le répertoire web :

    php bin/console assets:install web

Puis créez les tables correspondantes au schéma Doctrine :

    php bin/console doctrine:schema:update --dump-sql
    php bin/console doctrine:schema:update --force

Ajoutez les fixtures :

    php bin/console doctrine:fixtures:load



## Et voilà !
