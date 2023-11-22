# Workshop Ruby\Python

Tout d'abord vous devriez choisir sur quelle langage vous voulez partir! On est la pour vous aidez si vous savez pas du tout sur quoi partir :)

Une fois choisit, suivez les étapes d'installation du langage choisit:

## Python
Pour voir si vous avez Python3 déjà installer:  
**python3 —version**

Fedora:  
**sudo dnf install python3** 
 
Ubuntu:  
**sudo apt-get update**  
**sudo apt-get install python3**

## Ruby
Pour voir si vous avec Ruby déjà installer:  
**ruby —version**

Fedora:  
**sudo dnf install ruby**

Ubuntu:  
**sudo apt-get update**  
**sudo apt-get install ruby-full**

# Exercices
Nous allons passé maintenant à la découverte du langage que vous avez choisit. Chaque exercice à pour titre la notion que vous vouyez dans l'exercice. Bon courage à vous!!!  

**Attention chaque exercice doit être dans des fonctions!**  

### Exercice 1: Variables + Opérations 
Nous voulons que vous créez un personnage type avec sa taille, son âge, sa taille et son année de naissance que vous devez calculer avec son âge et l’année actuelle. Nous voulons que vous affichez toutes ces infos dans votre terminal:  

*Affichage attendu:* 
``` 
Nom: (nom_personne)  
Âge: (age_personne)  
Taille: (taille_personne en mètre -> avec précision 2 chiffres après la virgules)  
Il est donc née en (année_de_naissance_personnage)  
```


### Exercice 2: Opérations mathématiques 
Créez deux variables a et b et attribuez-leur des valeurs numériques.  

- Additionnez a et b -> stockez le résultat dans une variable nommez « somme »
- Soustrayez a et b -> stockez le résultat dans une variable nommez « difference »
- Multipliez a et b -> stockez le résultat dans une variable nommez « produit »
- Divisez a et b -> stockez le résultat dans une variable nommez « quotient »
Affichez tous les résultats  

### Exercice 3: Boucle for + Conditions
Tom est actuellement à un vide-grenier et il aimerait acheté des jeux anciens. Il a une liste précis de ce qu’il veut acheter. Vous devez l’aidez à choisir les jeux qu’il peut se permettre en fonction de la quantité d’argent qu’il a réussi à mettre de côté. Voici la liste des jeux et leurs prix:  
```
jeux = {
    "Mario Kart": 50,
    "Zelda: Breath of the Wild": 60,
    "Minecraft": 30,
    "Super Smash Bros": 55,
    "Animal Crossing": 45
}
```

Votre fonction prendra en paramètre l’argent que Tom a et vous afficherez le nom et le prix du jeu si Tom peut se l’acheter. A la fin vous affichez le nombre de jeu que Tom a pu acheté et l’argent qu’il lui reste.

### Exercice 4: Classes
Vous allez maintenant construire un jeu video où les joueurs ont des caractéristiques telles que leur nom et leur score. Vous allez créer une classe **«Joueur»** pour représenter un joueur dans le jeu.  
Vous devez stocker le nom du joueur et son score qui changera pendant le programme.
Vous auriez une fonction nommée **«afficher_details»** qui permettra d’afficher les détails du joueurs (nom + score).  

Créez une instance de la classe Joueur avec le nom **"Alice"** et un score initial de 0, et une autre instance avec le nom **"Bob"** et un score initial de 100. Afficher dans un premier lieu les détails des joueurs.

Alice et Bob jouent a votre jeux donc gagne des points sur leur score. Il va falloir créer une fonction qui prend en paramètre l’augmentation qu’ils vont avoir sur leur score. Et vous devrez le mettre à jour.

Ensuite rappelez la fonction pour détails les infos du joueurs pour voir si la variable a bien été changé.  

### Exercice 5: Double tableau:
Supposons que vous gérez une équipe de football et que vous souhaitez suivre les scores des matches de votre équipe au fil de la saison. Vous allez créer un tableau bidimensionnel pour stocker ces scores.  
Créez un double tableau appelé scores pour stocker les scores de chaque match de la saison. Chaque ligne du tableau représentera un match et contiendra les scores de votre équipe et de l'équipe adverse.  
*Par exemple:*
```
scores = [[2, 1],[3, 0]]
```

Ajoutez au moins 5 matches à votre tableau en utilisant des scores différents et pas en brut vous devez trouvé des méthodes pour ajouter des éléments au tableau.

Créer une fonction qui vous permet d’afficher tous les scores des maths et un message qui indique le numéro du match

***A la suite vous devez faire deux doubles tableaux:***  
- 1ère double tableau qui prend que les matches que votre équipe à gagner
- 2ème double tableau qui prend toutes les matches qui ont perdu

Et afficher le nombre d’éléments que vous avez dans chaque tableau.  
Puis afficher quelle équipe a gagné la compétition.  

### Exercice 6: Dictionnaire
Créez une classe **«Livre»** avec un constructeur qui prend les paramètres suivants :  
- «title»
- «auteur»
- «annee_publication»
- «disponible»  
Stockez ces valeurs dans un dictionnaire où les clés sont les noms des attributs (« titre », « auteur », « annee_publication », « disponible »).

Ajoutez une fonction **«afficher_details»** à la classe **«Livre»** qui affiche les détails du livre en parcourant le dictionnaire et en affichant chaque paire clé-valeur.

Créez quatre instance de la classe **«Livre»** pour représenter des livres de votre choix en utilisant un dictionnaire pour stocker les informations.

Écrivez une fonction **«emprunter_livre»** qui prend le titre du livre en paramètre et met à jour la valeur associée à la clé **«disponible»** pour le livre emprunté. Écrire un message de succès si le livre et dispo. Et un message d’excuse si le livre n’est pas disponible.

Écrivez une fonction **«retourner_livre»** qui prend le titre du livre en paramètre et met à jour la valeur associée à la clé **«disponible»** pour le livre retourné.

### Exercice 7: Bistro-matic
Le but de cet exercice est d'écrire un programme qui affichera le résultat d'une expression mathématique évaluée. L'expression sera composée d'entiers infinis pouvant être exprimés dans n'importe quelle base.  
Le programme doit gérer les opérateurs suivants : +-*/%, parenthèses, priorités d'opération et erreurs de syntaxe, **mais pas les nombres flottants.**  
Exemple:  
```
echo ‘3+6’ | ./calc 0123456789 ‘()+-*/%’ 3 ; echo 9

echo ‘----++-6*12’ | ./calc 0123456789 ‘()+-*/%’ 11 | cat -e ; echo -72

echo ‘-(12*(13+15/5*(6/(12+14%(30%5+(10*25)-46)+16)-20)/43)*20)*(-(12-98*42)*(16+63-50/3))’ | ./calc 0123456789 ‘()+-*/%’ 84 | cat -e ; echo -744629760
```