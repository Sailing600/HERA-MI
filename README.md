# HERA-MI

Pour réaliser votre exercice je commence par créer deux machines virtuelles pour pouvoir y mettre docker et donc avoir par la suite des conteneurs dans deux réseaux distinct.


Pour pouvoir synchroniser les fichiers d’un conteneurs à l’autre je lie ces deux derniers par une connection ssh avec une authentification par clé ce qui permet au deux conteneurs d’être liés constamment.

Un repertoire est créer sur chaque conteneur pour pouvoir accueillir les différents fichiers.

Je clone les fichiers présent sur votre Repository Git via la commande git clone :

git clone https://github.com/hera-mi/test_material.git



Je créer ensuite un script scp pour pouvoir transférer les fichiers du répertoire du conteneurs C1 à C2 : 




Ensuite je créer un dockerfile pour pouvoir deployer le conteneur C3 contenant la base de données Mongo DB.
