# TP3
 
#INSTALL
pour installer les services on utilise les commandes suivants:

git clone https://github.com/Sarah0408/TP3/
./install.sh
cd Documents/
cd TP3
cd src

#Encrypt
Ce service ecrit la date de demarrage sur un fichier situe dans /var/log/encrypt/encrypt.out
Il ecrit un fichier de message chiffre chaque fois qu'il est lance.
POur l'activer ,tapez la commande suivante:

sh
Sudo systemctl start encrypt.service.

ensuite verifiez dans /var/log/encrypt/encrypt.out


#decrypt
Ce service decrypte un fichier et ercit le fichier dechiffre sur un fichier /var/log/decrypt/decrypt.out.

Pour verifier qu'il fonctionne, on saisit la commande

sh
sudo systemctl status decrypt.service

POur desinstaller le projet, on fait:
 sh
 cd ..
 cd ..
 ./
 uninstall.sh
 #pour tester , on tape les commandes suivants:
 cd Documents
 cd TP3
 cd resources
 ls
 nano toto.txt(C'est le fichier on ecrit la phrase ou texte qu'on designe de decrypter)
 sauvegarder
 cd ..
 ls 
 cd src
 python3 crypt.py ../resources/toto.txt ../results/crypted.txt(on aura notre texte crypter)
 python3 decrypt.py ../results/crypted.txt ../results/decrypted.txt(le texte sera decrypter)
