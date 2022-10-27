*Calculatrice sous le logiciel de circuits logiques [Logisim](https://fr.wikipedia.org/wiki/Logisim)*

Étapes:<br/>
-> Création d'un [afficheur à 7 segments](https://www.linternaute.fr/dictionnaire/fr/definition/afficheur-7-segments/): 4 bits en entrée (ici on va jusqu'à 1001, soit 9). En utilisant des portes **NON** et **ET**, on peut faire pour chaque cas.<br/>
![7segments](https://user-images.githubusercontent.com/116813446/198292428-6ef138a5-e7bf-40a2-bb5c-fc9805a39c51.PNG)<br/>
-> On construira des circuits pour additionner dans un cadre de démonstration (problème pour la soustraction), sinon on utilisera les modules intégrés au logiciel. Pour chaque fin d'addition/de soustraction, on mettra des sous-circuits **7-segments** avec affichages.<br/> 
-> On crée le circuit d'opération simple bit+bit+bit (le dernier bit pour la possible retenue), qui fait sortir le résultat et la retenue.<br/>
-> Règles d'addition de bits: 0+0=0 ; 0+1=1 ; 1+0=1 ; 1+1=0 retenue de 1 ; 0+0+0=0 et 1+1+1=1 retenue de 1.<br/>
-> On doit faire la conversion pour deux affichages: on prend un nombre allant jusqu'à 30 en binaire, on le divise par 10, le divise par 6, puis le somme avec le nombre entrée pour obtenir le résultat.<br/>
-> Maintenant on peut construire la démo (addition de 4 bits et 4 bits); on place des sous-circuits **bit+bit et retenue** à la chaîne.<br/>
-> Utilisation module soustraction dans le circuit suivant.<br/>
-> Après plusieurs recherches infructueuses, l'affichage 5 chiffres a pu être fait à partir du BCD (Binary Coded Decimal, soit Décimal Codé Binaire), qui permet cette conversion (sous-circuit add3 avec table de vérité, puis circuit en escalier).<br/>
-> La suite part du même principe.<br/>
![4bits4bitsaddition](https://user-images.githubusercontent.com/116813446/198297935-fbc2051d-cda0-480d-8651-8916a3f61566.PNG)



