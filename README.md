*Calculatrice sous le logiciel de circuits logiques Logisim*

Étapes:<br/>
-> Création d'un [afficheur à 7 segments](https://www.linternaute.fr/dictionnaire/fr/definition/afficheur-7-segments/): 4 bits en entrée (ici on va jusqu'à 1001, soit 9). En utilisant des portes NON et ET, on peut faire pour chaque cas.<br/>
![7segments](https://user-images.githubusercontent.com/116813446/198292428-6ef138a5-e7bf-40a2-bb5c-fc9805a39c51.PNG)<br/>
-> On construira des circuits pour additionner dans un cadre de démonstration (problème pour la soustraction), sinon on utilisera les modules intégrés au logiciel<br/> 
-> On crée le circuit d'opération simple bit+bit+bit (le dernier bit pour la possible retenue), qui fait sortir le résultat et la retenue.<br/>
-> Règles d'addition de bits: 0+0=0 ; 0+1=1 ; 1+0=1 ; 1+1=0 retenue de 1 ; 0+0+0=0 et 1+1+1=1 retenue de 1.<br/>
-> On doit faire la conversion pour deux affichages: on prend un nombre allant jusqu'à 30 en binaire, on le divise par 10, le divise par 6, puis le somme avec le nombre entrée pour obtenir le résultat.

