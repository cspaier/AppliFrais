# ApplisFRais

Application web de gestion des frais du laboratoire GSB.

## Déploiement local
Executer les scripts `sql` puis servir le dossier `www` par un serveur web (apache).

- Pour executer les scripts sql il faudra tout d'abord aller dans le `cmd`.
- Dans le cmd, ce placer à l'emplacement où se trouve le site avec la commande `cd`.
- Une fois placer à l'emplacement souhaité, executer la commande `mysql -u root -p` puis appuyer sur entrer.
- Après cela taper les commandes `source gsbfrais_bduser.sql`, puis `source gsbfrais_structure.sql`, puis `source gsbfrais_data.sql`.

Voila, maintenant tout devrai fonctionner.


## Mise en production
On veillera à changer le mot de passe de l'utilisateur `sql` dans `ScriptsSQL/gsbfrais_bduser.sql` et dans le fichier `config.php`

Seul le dossier `www` doit être servi par le serveur web.