# Introduction à Python.

- *Table des matières*

# **Légende du cours**

---

# Ceci est un titre majeur

## Ceci est un sous-titre

**Ceci est un point important**

<aside>
📝 Ceci est un exemple single line

</aside>

<aside>
⚠️ Ceci est une mise en garde

</aside>

<aside>
💡 Ceci est un conseil

</aside>

[Ceci est un texte avec un lien vers un site ressource](https://www.w3schools.com/python/default.asp)

**Exemple**

```python
# Ceci est un exemple de code
```

# Introduction

---

## Qu’est-ce que le python ?

Le python est un langage de programmation très populaire créé au début des années 90.

**Il est utilisé majoritairement pour :**

- Le développement web (backend / côté serveur).
- La création d’applications.
- Les mathématiques (modélisation, statistiques, machine learning, etc.).

**Qu’est-ce que le python peut faire ?**

- Le python peut être utilisé sur un serveur pour créer des applications web.
- Il peut être utilisé pour connecter des bases de données, et peut être utilisé pour lire et modifier des fichiers.
- Le python est souvent utilisé pour tenir des grands jeux de données et appliquer des fonctions mathématiques complexes.
- Et enfin, il peut être utilisé pour faire du prototypage, et de la création d’application prêtes pour le déploiement.

**Ce qu’il faut savoir :**

- La version majeure la plus récente de python est `Python 3` (py3) , celui qu’on va utiliser pendant ce cours d’introduction. Même si `Python 3` (py2) est très populaire mais plus maintenu.

**La syntaxe du python par rapport à d’autres langages de prorammation**

- Le python a été designé pour la lisibilité et partage de nombreuses similarités avec l’anglais, tout en étant influencé par les mathématiques.
- Le python utilise de **nouvelles lignes** pour compléter une commande, comparé à d’autres langages qui utilisent des point-virgule `;` ou des parenthèses `(` `)`.
- Le python utilise l’**indentation** et les espaces vides pour définir la portée, le cadre d’une **fonction**, d’une **boucle** ou d’une **classe**. La majorité des langages utilisent les accolades `{`  `}` pour cela. Ainsi, au sein des boucles, on utilise l’indentation au lieu de *begin* et de *end*.

## Pour bien commencer

---

La majorité des PC et des Mac auront Python de préinstallé.

- La dernière version est la `3.10` (`3.11` en version bêta) mais généralement, on en est à `3.9.12` (surtout sur Mac).
- Pour vérifier si vous avez python d’installé sur votre PC ou Mac, lancez un terminal de commandes et tapez la commande suivante :

```bash
python --version
```

Si la commande n’est pas trouvée, vous pouvez installer python sur leur site : 

[Welcome to Python.org](https://www.python.org/)

## Vos premières lignes de code

---

### Explications

Le python est un langage de programmation interprété, ce qui veut dire que en tant que développeur, vous écrivez des fichiers en python (`.py`) dans un éditeur de fichiers, puis vous utilisez l’interpréteur pour les exécuter.

Voici la démarche :

```bash
python miashsvie.py
```

Où `miashsvie.py` est le nom de votre fichier.

### Exemple

Créons notre premier fichier, que nous allons appeler `miashsvie.py`. Cela peut être fait dans n’importe quel éditeur de texte (Ou des applications comme [Atom](https://atom.io), [PyCharm](https://www.jetbrains.com/fr-fr/pycharm/download/#section=windows), [Spyder](https://www.spyder-ide.org) ou [Visual Studio Code](https://code.visualstudio.com/#alt-downloads) par exemple).

Dedans, écrivez :

```python
print("Go les MIASHS")
```

Sauvegardez votre fichier, ouvrez votre terminal de commandes dans le dossier ou vous avez enregistré le fichier et exécutez :

```python
python miashsvie.py
```

La sortie de cette commande devrait être :

```python
Go les MIASHS
```

Félicitations ! Vous avez écrit et exécuté votre premier programme en `Python` !

## Le terminal de commandes en Python

---

Pour tester une *petite quantité* de code en python, il est parfois préférable et plus rapide de l’exécuter dans le terminal en python.

Pour cela écrivez la commande suivante dans votre terminal de commandes :

```bash
python
```

*(Oui oui, aussi simple que ça)*

Depuis ici, vous pourrez écrire n’importe quoi en python, même l’exemple que nous avions fait plus tôt.

```python
# C:\Users\Your Name>python
# Python 3.9.7 (tags/v3.9.7:1016ef3, Aug 30 2021, 20:19:38) [MSC v.1929 64 bit (AMD64)] on win32
# Type "help", "copyright", "credits" or "license" for more information.

>>> print("Go les MIASHS")
Go les MIASHS
```

Dès que vous avez terminé avec le console Python, vous pouvez écrire la commande suivante pour la quitter :

```python
exit() # Il s'agit d'une fonction, ne pas oublier les parenthèses
```

# Fonctionnalités

---

## Librairies (As)

---

### **Objectif**

Elles fournissent des outils et fonctions avancées pour ce qu'on souhaite faire : ouvrir des fichiers avec des extensions particulières, visualiser des données, effectuer des tests statistiques et de performances, modéliser des données cérébrales, réaliser des cartes, etc.

### **Installation**

Il suffit d’ouvrir le terminal (comme vu précédemment) et d’utiliser `pip install` (possible pour des versions `Python` ultérieures à 3.4) suivi du nom de la librairie.

```bash
pip install NomLibrairie
```

Si on souhaite une version particulière, on peut la stipuler avec `pip`.

```bash
pip install NomLibrairie==1.4 
```

Si on souhaite une version ultérieure à une version spécifique, on peut aussi le préciser.

```bash
pip install NomLibrairie>=1.4 
```

Pour mettre à jour une librairie (qui sont souvent mises à jour car Python est en pleine expansion).

```bash
pip install --upgrade NomLibrairie
```

### **Méthode**

On utilise `import` avant de préciser le **nom** de la librairie (comme les packages sur `R`) qu’on souhaite utiliser, et `as` suivi de comment on veut les **appeler** dans le reste du programme (pour éviter d’avoir à réecrire un nom très long).

```python
import NomLibrairie as NomRaccourci
```

**Exemple**

```python
import numpy as np
```

On peut aussi importer une fonction spécifique d’une librairie en utilisant `from`.

**Exemple**

```python
from numpy import asarray
```

### **Les indispensables**

Manipuler et traiter des [petits et moyens tableaux](https://datascientest.com/pandas-python-data-science) de données.

```python
import pandas as pd
```

Manipuler et traiter des [grands tableaux](https://courspython.com/apprendre-numpy.html) de données.

```python
import numpy as np
```

Visualiser [graphiquement](https://openclassrooms.com/fr/courses/4452741-decouvrez-les-librairies-python-pour-la-data-science/4740942-maitrisez-les-possibilites-offertes-par-matplotlib) des données. 

```python
import matplotlib.pyplot as plt
```

Visualiser [graphiquement](https://openclassrooms.com/fr/courses/4452741-decouvrez-les-librairies-python-pour-la-data-science/5559011-realisez-de-beaux-graphiques-avec-seaborn) (complète `matplotlib`).

```python
import seaborn as sns
```

Évaluer les [performances](https://scikit-learn.org/stable/modules/model_evaluation.html) de classification : si l'IA fait bien son travail, et comment.

```python
from sklearn import metrics
```

## Variables (As)

---

Comme pour la plupart des langages, le `Python` permet de manipuler différents types de variables : 

- Booléen (`bool`) : Vrai / Faux.
- Entier (`int`).
- Texte (`str`).
- Liste (`list`).
- Réel (`float`).

Contrairement à certains langages (#Pascal), le type de variable est précisé lorsqu’on attribue une valeur à la variable.

Ainsi, si on stocke le nombre 8 dans la variable `dinosaure`, elle sera du type `**int**`.

```bash
dinosaure = 8
print(type(dinosaure))
# Ce qui affiche
>> int
```

Mais si on stocke “vive la MIASHS” dans la variable `dinosaure`, elle sera du type `**str**`.

```bash
dinosaure = "vive la MIASHS"
print(type(dinosaure))
# Ce qui affiche
>> str
```

## Structures (As)

---

### Listes

**Créer une liste vide.**

```python
NomListe = list()
```

**Compléter la liste.**

```python
NomListe.append(Item1, Item2) # Les items peuvent être des nombres, du texte, etc.
# Par exemple
NomListe.append (3, "dinosaure", 34.6)
```

**Créer et remplir une liste.**

```python
NomListe = ["dinosaure", "pancakes"] # Liste de mots
NomListe = [1, 2, 3] # Liste de chiffres
NomListe = [17, "pirouette", 3, "cacahouète"] # Liste mixte
NomListe = range(10) # Liste de chiffres de 0 à 9
NomListe = range(1, 10, 2) # Liste de chiffres de 1 à 10 en allant de 2 en 2
```

**Mesurer sa longueur.** 

```python
LongueurListe = len(NomListe)
```

**Accéder à un élément.**

```python
Element = NomListe[3] #4ème élément (l'index commence à 0)
```

**Liste de listes.**

```python
MegaListe = [Liste1, Liste2, Liste3]
```

**Accéder à un élément d’une liste de listes.**

```python
Element = MegaListe[2][0] #3ème liste, 1er élément (l'index commence à 0)
```

### Tableaux

Ils permettent de stocker, visualiser et manipuler les jeux de données facilement grâce à des `[DataFrame](http://www.python-simple.com/python-pandas/creation-dataframes.php)`.

**Import.**

```python
from pandas import DataFrame
```

**Sélectionner des colonnes / lignes particulières.**

Par indices (lignes, colonnes).

```python
df.iloc[0,5] # 1ère ligne, 6ème colonne
df.iloc [0:5, 0:3] # 1ère à 6ème lignes et 
df.iloc[:, 0:3] # toutes les lignes et 1ère à 4ème colonnes
df.loc[:, 'NomColonne'] # toutes les lignes et colonne "NomColonne"
```

Par position.

```python
df.head(5) # Afficher les 5 premières lignes
df.head(10) # Afficher les 10 premières lignes
```

**Modifier le contenu.**

🚧🚧🚧🚧🚧🚧 AS 🚧🚧🚧🚧🚧🚧 

df.columns.str.lower()

équivalent factorize() sur R —>  [https://pandas.pydata.org/docs/reference/api/pandas.factorize.html](https://pandas.pydata.org/docs/reference/api/pandas.factorize.html)

voir tout ça même avec panda (même si df >>>)

🚧🚧🚧🚧🚧🚧 AS 🚧🚧🚧🚧🚧🚧 

## Fonctions (As)

---

### Fonctions utiles

**Importer un fichier .csv (comptatible avec `Excel`).**

```python
from pandas import read_csv
```

On précise :

- Le *fichier* souhaité (ou son *[chemin](https://www.pcastuces.com/pratique/astuces/5995.htm)* s’il se situe dans un répertoire différent).
- S'il possède des *entêtes* (ici, aucune).
- La colonne qui sert d'*index*, c'est-à-dire de référence, du style un numéro unique, comme les clés en BDD (ici, la première colonne, donc 0, sert d'index).
- Le type de *séparateur* *de* *données* (par défaut : `,`).
- Le type de *séparateur* *décimal* (par défaut : `.`, souvent `,` pour des jeux de données européens).

```python
data = read_csv('NomFichier.csv', header = 0, index_col = 0, sep= ';', dec = ',')
```

Il est donc important d’ouvrir le fichier avant pour vérifier ces informations

À noter qu’on peut aussi importer un jeu de données directement depuis le web. 

```python
data = read_csv('https://UrlDuFichierFinissantPar.csv', header = 0, index_col = 0, sep = ';', dec = ',')
```

**Afficher du texte et des variables.**

```python
print (”Go les MIASHS”)
```

Ce qui nous donne :

```bash
Go les MIASHS
```

On peut aussi mélanger du texte brut avec des variables.

```python
prenom = "Stéphane"
nom = "Chrétien"
print ("Directeur de l'UFR :", prenom, nom)
```

Ce qui nous donne :

```bash
>> Directeur de l'UFR : Stéphane Chrétien
```

**Visualiser les données.**

Cela permet de voir rapidement le type de données et leur répartition. Cela permet d’orienter les décisions concernant les traitements et tests à effectuer.

```python
pyplot.plot(NomDonnées)
pyplot.show()
```

🚧🚧🚧🚧🚧🚧 AS 🚧🚧🚧🚧🚧🚧 

```python
plt.hist(X)
```

```python
as_ordered()
```

```python
sort_values()
```

```python
sort()
```

🚧🚧🚧🚧🚧🚧 AS 🚧🚧🚧🚧🚧🚧 

### Créer une fonction

Il existe un large éventail de **fonctions prédéfinies**, mais il arrive qu’on ait besoin de réaliser régulièrement le même **ensemble de traitements**. Pour éviter d’abuser du copier-coller, on peut alors définir ses propres fonctions.

Pour ce faire, on utilise `def`, on **nomme** la fonction (utiliser un nom assez explicite, tout en évitant qu’il soit trop long si on y fait souvent appel). 

Puis, on précise s’il y a des variables en **entrée** (par exemple pour afficher des données, les tranformer, etc.). Il est possible qu’il n’y ait aucun paramètre en entrée (comme pour un compteur par exemple). 

On utilise les `:` pour préciser que le **bloc d’instructions** va suivre. On décrit ensuite les instructions après **indentation** (précise le début du bloc et la fin du bloc).

Enfin, on peut préciser des variables de **sortie** (si on effectue des calculs par exemple). De même, il se peut qu’il n’y ait pas de paramètres de sortie.

```python
def NomFonction (paramètre_1, paramètre_2, paramètre_3):
 
	# Instruction 1
	# Instruction 2
	# Instruction 3

	return sortie_1, sortie_2
```

On peut ensuite appeler cette fonction autant de fois qu’on le souhaite en spécifiant les paramètres soit directement en suivant l’ordre dans lequel ils ont été déclarés, soit dans un ordre différent en précisant les paramètres.

**Exemple**

```python
def CarteEtu (nom, prenom, numetu)

	print ("--- Carte étudiante ---")
	print ("Nom :", nom)
	print ("Prénom :", prenom)
	print ("Numéro étudiant :", numetu)
```

On peut alors soit appeler la fonction en précisant les variables en entrée en suivant le même ordre.

```python
CarteEtu (”Chrétien”, “Stéphane”, 219574)
```

Ce qui nous affiche  :

```bash
>> --- Carte étudiante ---
	 Nom : Chrétien
	 Prénom : Stéphane
	 Numéro étudiant : 219574
```

Mais si on ne se souvient plus de l’ordre, ou qu’on aime se rebeller, on peut préciser à quoi correspondent nos variables en entrée.

```python
CarteEtu (numetu = 219574, prenom = “Stéphane”, nom =”Chrétien”)
```

Ce qui nous affiche  :

```bash
>> --- Carte étudiante ---
	 Nom : Chrétien
	 Prénom : Stéphane
	 Numéro étudiant : 219574
```

## Opérateurs (Ben)

---

Les opérateurs sont utilisés pour réaliser des opérations sur des variables et des valeurs.

En `Python`, les opérateurs sont séparés dans différents groupes :

- Opérateurs arithmétiques.
- Opérateurs d’assignement.
- Opérateurs de comparaison.
- Opérateurs logiques.
- Opérateurs d’identité.
- Opérateurs d’appartenance.
- Opérateurs de comparaison (Bitwise).

### Opérateurs arithmétiques

Les opérateurs arithmétiques sont utilisés avec des valeurs numériques pour réaliser des opérations mathématiques courantes :

| Opérateur | Nom | Exemple |
| --- | --- | --- |
| + | Addition | x + y |
| - | Soustraction | x - y |
| * | Multiplication | x * y |
| / | Division | x / y |
| % | Modulo | x % y |
| ** | Exponentielle | x ** y |
| // | Division Euclidienne | x // y |

### Opérateurs d’assignement

Les opérateurs d’assignement sont utilisés pour assigner des valeurs à des variables.

| Opérateur | Exemple | Équivalence |
| --- | --- | --- |
| = | x = 5 | x = 5 |
| += | x += 5 | x = x + 5 |
| -= | x -= 5 | x = x - 5 |
| *= | x *= 5 | x = x * 5 |
| /= | x /= 5 | x = x / 5 |
| %= | x %= 5 | x = x % 5 |
| //= | x //= 5 | x = x // 5 |
| **= | x **= 5 | x = x ** 5 |

### Opérateurs de comparaison

Les opérateurs de comparaison sont utilisés pour comparer deux valeurs.

| Opérateur | Nom | Exemple |
| --- | --- | --- |
| == | Egal | x == y |
| |= | Non égal | x |= y |
| > | Plus grand que | x > y |
| < | Plus petit que | x < y |
| >= | Plus grand ou égal | x >= y |
| <= | Plus petit ou égal | x <= y |

### Opérateurs logiques

Les opérateurs logiques sont utilisés pour combiner des instructions conditionnelles.

| Opérateur | Description | Exemple |
| --- | --- | --- |
| and | Retourne true si les deux instructions sont vraies | x < 5 and x < 10 |
| or | Retourne true si l’une des deux instructions sont vraies | x < 5 or x < 4 |
| not | Inverse le résultat, retourne false si le résultat est true | not(x < 5 and x < 10) |

### Opérateurs d’identité

Les opérateurs d’identité sont utilisés pour comparer des objets, non pas s’ils sont égaux, mais si ils sont actuellement le même objet avec le même emplacement mémoire.

| Opérateur | Description | Exemple |
| --- | --- | --- |
| is | Retourne true si les deux variables sont le même objet | x is y |
| is not | Retourne true si les deux objets ne sont pas le même objet |  x is not y |

### Opérateurs d’appartenance

Les opérateurs d’appartenance sont utilisés pour tester si une séquence est présente dans un objet.

| Opérateur | Description | Exemple |
| --- | --- | --- |
| in | Retourne true si une séquence avec la valeur spécifiée est présente dans l’objet | x in y |
| not in | Retourne true si une séquence avec la valeur spécifiée n’est pas présente dans l’objet | x not in y |

### Opérateurs de comparaison (Bitwise)

Les opérateurs bitwise sont utilisés pour comparer des nombres binaires.

| Opérateur | Nom | Description |
| --- | --- | --- |
| & (et commercial) | AND | Définit chaque bit à 1 si les deux bits sont 1 |
| | (pipe) | OR | Définit chaque bit à 1 si l’un des deux bits est 1 |
| ^  | XOR | Définit chaque bit à 1 si uniquement l’un des deux bits est 1 |
| ~ (tilde) | NOT | Inverse tout les bits |

## Boucles & Conditions (Ben)

---

### **Conditions et instructions `If`**

Le python supporte les conditions logiques classiques provenant des mathématiques :

- Egal : `a == b`
- Non égal : `a != b`
- Inférieur à : `a < b`
- Inférieur ou égal à : `a <= b`
- Supérieur à : `a > b`
- Supérieur ou égal à : `a >= b`

Ces conditions peuvent être utilisés dans plusieurs méthodes, la plus commune des utilisations reste les conditions `if` et les boucles.

Une condition `if` est écrite en utilisant le mot clé `if`.

**Exemple**

```python
a = 33
b = 200

if b > a:
	print("b est plus grand que a")
```

Dans cet exemple, nous utilisons deux variables : `a` et `b` qui sont utilisées par l’instruction if pour tester si `b` est plus grand que `a` , sachant que `a` est égal à `33` et que `b` est égal à `200`, nous savons que `200` est plus grand que `33`, nous écrivons donc que “b est plus grand que a”.

### Indentation

Le python se base sur l’indentation (une tabulation au début de la ligne), pour définir la portée du code. Les autres langages utilisent principalement les “curly-brackets” : `{ }` pour cette utilisation.

**Exemple (qui génèrera une erreur)**

```python
a = 33
b = 200

if b > a:
print("b est plus grand que a") # Pas d'indentation, la portée n'est pas définie
```

### Elif

Le mot-clé `elif` est plus communément utilisé comme `else if` dans les autres langages. C’est la façon de dire “Si la condition précédente n’était pas vraie, alors essayer cette condition”.

**Exemple**

```jsx
a = 33
b = 33

if b > a:
	print("b est plus grand que a")
elif a == b:
	print("a et b sont égaux")
```

### Else

`Else` est utilisé dans le cas ou la ou les conditions précédentes ne sont pas remplies

**Exemple**

```jsx
a = 200
b = 33

if b > a:
	print("b est plus grand que a")
elif a == b:
	print("a et b sont égaux")
else:
	print("a est plus grand que b")
```

### And

Le terme `and` est un opérateur logique, et utilisé pour combiner des instructions conditionnelles.

**Exemple**

```jsx
a = 200
b = 33
c = 500

if a > b and c > a:
	print("Les deux conditions sont vraies")
```

### Or

`or` est un opérateur logique utilisé comme `and` pour combiner des instructions conditionnelles.

**Exemple**

```jsx
a = 200
b = 33
c = 500

if a > b or a > c:
	print("Au moins une des conditions est vraie")
```

### Pass

Les instructions `if` ne peuvent pas être vides, mais si pour une raison vous avez un `if` sans contenu, utilisez l’instruction `pass` pour empêcher la génération d’erreurs.

**Exemple**

```jsx
a = 33
b = 200

if b > a:
	pass
```

### Boucles `While`

Avec les boucles `while`, nous pouvons éxecuter une suite d’instructions tant qu’une condition est vraie.

**Exemple**

```jsx
i = 1
while i < 6:
	print(i)
	i += 1
```

<aside>
⚠️ Pensez à incrémenter (+1) i, sinon la boucle sera infinie.

</aside>

Les boucles `while` requièrent des variables déjà déclarées, c’est pour cela que dans cet exemple nous déclarons `i` et définissons sa valeur à `1`.

### Break

L’instruction `break` est utilisée pour stopper les boucles, même si la condition active est vraie.

**Exemple**

```jsx
i = 1
while i < 6:
	print(i)
	if i == 3:
		break
	i += 1
```

### Continue

Avec l’instruction `continue` nous pouvons stopper l’itération actuelle, puis continuer avec la suivante

**Exemple**

```python
i = 0
while i < 6:
	i += 1
	if i == 3:
		continue
	print(i)
```

### Else

Comme pour les `if`,  nous pouvons exécuter un bloc de code quand la condition n’est plus vraie.

**Exemple**

```python
i = 1
while i < 6:
	print(i)
	i += 1
else:
	print("i n'est plus plus petit que 6")
```

### Les Boucles `For`

Une boucle `for` est utilisée pour itérer sur une séquence, qui peut être une liste, un dictionnaire, un string etc.

Ce type de boucle ressemble moins aux boucles `for` d’autres langages. Elle fonctionne plus comme une méthode d’itération trouvée dans les langages de programmation orienté objet.

Avec la boucle `for` nous pouvons éxecuter une suite d’instructions, pour chaque item dans une liste, une suite ou autre...

**Exemple**

```python
fruits = ["pomme", "banane", "cerises"]
for x in fruits:
	print(x)
```

La boucle `for` ne nécessite pas d’indexer une variable déclarée au préalable.

### Boucler dans une chaîne de caractères (String)

Même les chaîne de caractères (String) sont des objets itérables, ils contiennent une séquence de caractères :

**Exemple**

```python
for x in "banane":
	print(x)
```

### Break

Avec l’instruction `break` nous pouvons stopper une boucle avant qu’elle ne soit passée par tout les items :

**Exemples**

```python
fruits = ["pomme", "banane", "cerise"]
for x in fruits:
	print(x)
	if x == "banane":
		break
```

```python
fruits = ["pomme", "banane", "cerise"]
for x in fruits:
	if x == "banane":
		break
	print(x)
```

### Continue

L’instruction `continue`est utilisée pour stopper l’itération actuelle et continuer à la prochaine : 

**Exemple**

```python
fruits = ["pomme", "banane", "cerise"]
for x in fruits:
	if x == "banane":
		continue
	print(x)
```

### La fonction `range()`

Pour boucler dans un suite de code un certain nombre de fois, nous pouvons utiliser la fonction `range()`.

La fonction `range()` retourne une séquence de nombres, démarrant de 0 par défaut, et s’incrémentant par 1 (par défaut), et se termine par le nombre spécifié.

**Exemple**

```python
for x in range(6):
	print(x)
```

<aside>
⚠️ Notez que `range(6)` comprend les valeurs de 0 à 5 et non de 0 à 6, c’est le nombre d’itérations.

</aside>

La fonction `range()` commence par défaut à 0 comme valeur de départ. Cependant il est possible de spécifier une valeur de départ en ajoutant un paramètre : `range(2, 6)`, ce qui veut dire les valeurs de 2 à 6 (N’incluant pas 6)

**Exemple**

```python
for x in range(2, 6):
	print(x)
```

Il est aussi possible de spécifier une valeur d’incrément (qui est par défaut 1) en ajoutant un troisième paramètre : `range(2, 30, 3)` : 

**Exemple**

```python
for x in range(2, 30 ,3):
	print(x)
```

### Else

L’instruction `else` dans une boucle `for` permet de spécifier un bloc de code qui sera exécuté quand la boucle se termine :

**Exemple**

```python
for x in range(6):
	print(x)
else:
	print("Boucle terminée")
```

<aside>
⚠️ Notez que le bloc `else` ne sera pas exécuté si la boucle est stoppée par un `break`

</aside>

**Exemple**

```python
for x in range(6):
	if x == 3: break
	print(x)
else:
	print("Boucle terminée")
```

### Pass

Les boucles `for` ne peuvent pas être vides, mais si pour une raison vous avez une boucle `for` avec aucun contenu, insérez l’instruction `pass` pour éviter les erreurs.

**Exemple**

```python
for x in [0, 1, 2]:
	pass
```

## Graphiques (As)

---

## Machine Learning (Ben / As)

---

deep L

boosting

RF

PyTorch (what, why, how)

sklearn

[https://www.numerical-tours.com/python/](https://www.numerical-tours.com/python/)

## Statistiques (As)

---

### Statistiques descriptives

🚧🚧🚧🚧🚧🚧 AS 🚧🚧🚧🚧🚧🚧 

```python
describe()
```

sum()

mean()

median()

var()

std()

round()

exemple mean(X).round()

df.describe()

Etc.

🚧🚧🚧🚧🚧🚧 AS 🚧🚧🚧🚧🚧🚧 

### Statistiques inférentielles (tests)

🚧🚧🚧🚧🚧🚧 AS 🚧🚧🚧🚧🚧🚧 

Cf. fiche (retaper) 

[Fiche 2 - Tests.pdf](Cours%20Python%20-%20Stagiaires%20e25f1aa341f84823acfd826c91f79fd5/Fiche_2_-_Tests.pdf)

🚧🚧🚧🚧🚧🚧 AS 🚧🚧🚧🚧🚧🚧 

# Ressources

---

[Exercices](https://drive.protonmail.com/urls/0093XY42Y4#0dEUb8Z5FZB6) (énoncés et corrigés) par [Miguel Palencia-Olivar](https://github.com/mpalenciaolivar).

[Ressource](https://www.w3schools.com/python/) très complète d’aide et tutos.

[Notebooks](https://www.numerical-tours.com/python/) explicatifs (Machine Learning, optimisation, ondelettes, etc.)

[CM.pdf](Cours%20Python%20-%20Stagiaires%20e25f1aa341f84823acfd826c91f79fd5/CM.pdf)