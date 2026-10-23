TP Terminal

**Étape 1**

>Afficher le chemin du dossier courant:<br>
pwd

>Afficher son contenu :<br>
ls

>Afficher son contenu avec les fichiers cachés :<br>
ls -a

>Afficher son contenu en version longue (sans fichiers cachés) :<br>
ls -l

>Afficher son contenu en version longue avec fichiers cachés : <br>
ls -la

>Afficher aide de la commande : <br>
man ls

>Se déplacer dans dossier documents : <br>
cd ./documents

**Étape 2**

>Créez le dossier station-meteo : <br>
mkdir station-meteo, 

>Dans ce dossier créez un dossier brouillon et son sous-dossier data :<br>
cd ./station-meteo, <br>
mkdir -p brouillon/data

>créez en une seule commande les dossiers src , tests et docs à la racine de station-meteo : <br>
mkdir src tests docs

>créez dans brouillon un fichier main.py contenant la ligne print("Station météo prête") : <br>
touch main.py <br>
echo "print('Station météo prête')" > main.py
-> pour le faire sans aller dans le dossier brouillon :<br>
echo "print('Station météo prête')" > brouillon/main.py


>déplacez main.py dans src , puis le dossier data et son contenu à la racine de station-meteo : <br>
mv main.py ../  <br>
mv main.py src/ <br><br>
sans etre dans brouillon : <br>
mv brouillon/main.py ./src/
mv ./brouillon/data ./


>supprimez le dossier brouillon : <br>
rm -r brouillon

>exécutez src/main.py avec Python : <br>
python3 main.py<br><br>
sans etre dans src:<br>
python3 src/main.py


**Étape 3**

>créez fichier1.txt contenant Bonjour ! et fichier2.txt contenant Je m'appelle <votre prénom><br>
touch fichier1.txt <br>
echo "Bonjour " > fichier1.txt <br>
touch fichier2.txt <br>
echo "Je m'appelle Shirel " > fichier2.txt

>créez resultat.txt en concaténant les deux fichiers, puis affichez-le<br>
cat fichier1.txt fichier2.txt > resultat.txt <br>
cat resultat.txt


>ajoutez la ligne Fin du test. à la fin de resultat.txt sans effacer son contenu<br>
echo "Fin du test." >> resultat.txt 

>copiez resultat.txt en resultat_sauvegarde.txt<br>
cp resultat.txt resultat_sauvegarde.txt


**Étape 4**

>Affichez la liste des dernières commandes tapées. <br>
history

>Retrouvez une commande précédente avec le clavier, sans la retaper.<br>
En utilisant les flèche du clavier

>Depuis Documents , retrouvez tous les fichiers .py contenus dans station-meteo .<br>
find . -name "*.py"
