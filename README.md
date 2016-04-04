Installer Symfony sur linux :

sudo curl -LsS https://symfony.com/installer -o /usr/local/bin/symfony
sudo chmod a+x /usr/local/bin/symfony

---

créer un nouveau repertoire dans le /var/www/html :

symfony new nom_du_projet

---

Generer un Bundle :

php bin/console doctrine:database:create

php bin/console generate:bundle

entrer

mettre un nom de bundle

entrer

entrer

entrer

---

Generer une entité :

php bin/console generate:doctrine:entity

Nom_du_Bundle:Coach

entrer

nom du champ
type de champ
entrer
entrer

entrer (si plus de champ a ajouter)

---

Generer un Create Remove Update Delete :

php bin/console doctrine:generate:crud

''Reprendre le nom du Bundle'':Coach

yes

entrer

entrer

entrer

---

Mettre à jour la base de donnée :

php bin/console doctrine:schema:update --force

---

Voir le formulaire sur nom_du_repertoire/web/app_dev.php/coach/new
