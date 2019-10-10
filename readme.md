Algo & Poo with TypeScript
===

<h2>Jour 1</h2>

**MasterClass**
[Algo poo ts](https://fr.slideshare.net/mohamedElbabili/algo-poo-ts-180382848)

**jouons un peu avec les fonctions, boucles, conditions, bref des algos quoi !**

1.1 Ajouter dans IdeaProjects, un repo TPTS par ex, ajoutez-y un fichier game.ts puis écrire un programme demandant à l'utilisateur s'il souhaite jouer à notre jeu, si non alors sortir du programme, si oui, alors proposer de saisir un chiffre entre 1 et 100 et dire à chaque itération si le chiffre est plus petit ou plus grand... une fois le chiffre trouvé, sortir avec un message : vous avez trouvé en x coups !

1.2 Mettez en oeuvre un moyen de répéter le jeu autant de fois que le joueur souhaite

1.3 Que faites vous si l'utilisateur saisie de mauvaises valeurs ?

1.4 Automatiser l'execution via un fichier de configuration "tsconfig.json"

NB : Attention, vous devez tourner dans votre équipe, cad qu'au bout de 15 minutes, prenez la place du dev à votre droite.

**class les objets !**

2.1 : Ajouter dans un autre fichier (town.ts) une première classe Ville avec pour attributs (à traduire dans la langue de shake) public nom, pays, nbHabitants, définir 1 constructeur. Après quoi, instancier votre classe pour obtenir le résultat suivant : toulouse = new Town("TOULOUSE" , "FRANCE" , 500000); répétez l'instanciation de votre classe avec plusieurs villes puis afficher les attributs de chaque ville.

2.2 : Toujours dans votre classe, mettez en place vos accesseurs pour empecher l'utilisateur de changer vos attributs sans votre approbation, par ex, pour empecher l'usr de faire n'importe quoi : toulouse.nbHabitants = -200. Faites les tests nécessaires ici.

2.3 : Créer une méthode pour afficher les attributs d'une ville tel que toulouse.display() aura pour résultat : <ville de TOULOUSE en FRANCE avec 500000 habitants>

2.4 : Ajouter maintenant une méthode toString qui aura vocation de renvoyer le contenu de l'objet sous forme de chaine de caractère tel que console.log(toulouse.toString()) affiche le même résultat que toulouse.display();

2.5 : Trouver un moyen de compter le nombre d'instances de votre classe Town.

2.6 : Dans un nouveau fichier(person.ts), ajouter la classe Person avec pour attributs nom, prénom, âge, adresse et une méthode d'affichage comme vu précédemment.

<h2>Jour 2</h2>

**Composition, héritage & interface : Modules**

3.1 : Ajouter un Repo TPModule puis installer FuseBox, ajouter un fichier de config fuse.js...
[Installation · FuseBox](https://fuse-box.org/docs/getting-started/installation)

3.2 : Ajouter dans ce repo les fichiers person.ts et town.ts puis modifier votre classe Person en rajoutant l'attribut cityBirth qui est un objet de type Town (export), tester le tout avant de passer à la suite.

3.3 : Ajouter une classe Capital qui hérite de la classe Town avec comme particularité d'avoir un monument. En effet, Paris est une Ville avec un monument la tour Eiffel, Tester en instanciant des personnes qui habitent des capitales. Utiliser la méthode toString pour obtenir le résultat suivant :
console.log(andy.toString()); ---> Mc Dowell Andy 61 carnaby street Londres England 10000000 Big Ben

3.4 : Chaque ville a un programme écologique plus ou moins important avec des points imposés par l'état aussi trouver un moyen ici de représenter ce programme.

3.5 : Ecrire la classe Employe qui hérite de Person tel qu'un Employé est une Personne avec comme particularité d'être dans une entreprise et de bénéficier d'un salaire, prévoir un attribut cityWork pour lieu ou ville de travail, le tout en vue d'obtenir le résultat ci-dessous :

      let alabama = new Town("Alabama","Usa",1000000);     //ville de naissance
      let cupertino = new Town("Cupertino","Usa",450000);  //ville de travail
      let tim = new Employee("Cook" , "Tim" , 58 , "Palo Alto" , alabama , "Apple" , 250000 , cupertino);
      
      console.log(tim.toString());
      
      name:Cook | firstName:Tim | age:58 | address:Palo Alto | city Birth [name:Alabama | state:Usa | number of inhabitants:1000000] company:Apple | salary:250000 | working town [ name:Cupertino | state:Usa | number of inhabitants:450000]

3.6 : Petit programme de simulation d'une boutique en ligne offrant la possibilitée donc d'inter agir avec l'utilisateur
   lui permettant de voir une liste de produits dont il pourra constituer son caddy puis passer commande.
   L'utilisateur doit pouvoir donc : voir la liste des produits, le contenu de son caddy, ajout ou suppression de produits...

**Conlusions sur Algo & Poo avec TypeScript**

**RAPPELS SUR LES CONSIGNES**

++ Prenez l'habitude de créer de nouveaux repo par thématique ou TP

++ Vous devez commenter vos codes et les faire relire par vos pairs idéalement

++ Vos programmes doivent précisemment répondre aux besoins exprimé

++ respecter les règles d'écriture de code et de fichier (maj-min)

++ Les noms de classe, attributs, méthodes/fonctions et variables doivent être en anglais, suffisamment explicite et compréhensible de tous

++ attention à l'indentation

++ tester et(ou) mettre en oeuvre des tests unitaires

++ utiliser Git & Github en mode console ou via votre ide

++ Une fois tous ces critères respectés, vous pouvez mettre votre repo sur github et partager le lien avec vos formateurs
