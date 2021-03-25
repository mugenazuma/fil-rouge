                            ***Algorithme***
*******************************************************

                            Les variables

                            PARTIE 1
                            Enonce des Exercices




Exercice 1.1
Quelles seront les valeurs des variables A et B après exécution des instructions suivantes ?

résultat:

A=3
B=4

Exercice 1.2
Quelles seront les valeurs des variables A, B et C après exécution des instructions suivantes ?

résultat:

A=2
B=3
C=1

Exercice 1.3
Quelles seront les valeurs des variables A et B après exécution des instructions suivantes ?

résultat:

A= 10
B= 2

Exercice 1.4
Quelles seront les valeurs des variables A, B et C après exécution des instructions suivantes ?

résultat:

A= 13
B= 13
C= 13

Exercice 1.5
Quelles seront les valeurs des variables A et B après exécution des instructions suivantes ?

résultat:

A= 2
B= 2

Exercice 1.6
Plus difficile, mais c’est un classique absolu, qu’il faut absolument maîtriser : écrire un algorithme permettant 
d’échanger les valeurs de deux variables A et B, et ce quel que soit leur contenu préalable.

résultat:

A ← C
B ← A
C ← B

Exercice 1.7
Une variante du précédent : on dispose de trois variables A, B et C. Ecrivez un algorithme transférant à B la valeur de A, à C 
la valeur de B et à A la valeur de C (toujours quels que soient les contenus préalables de ces variables). 

résultat:

B ← A
C ← B
A ← C

Exercice 1.8
Que produit l’algorithme suivant ?

C ← "435" ("423"+"12")

Exercice 1.9
Que produit l’algorithme suivant ?

C ← "42312" ("423"&"12")

**********************************************************************************************************************************

                                                    Partie 2
                                                Lecture et Ecriture


Exercice 2.1
Quel résultat produit le programme suivant ?

Résultat:

Ecrire Val = 231
Ecrire Double = 231*2= 462

*****************************

Exercice 2.2
Ecrire un programme qui demande un nombre à l’utilisateur, puis qui calcule et  affiche le carré de ce nombre.

Variables chiffre, calcul numériques

Début
ecrire "saisir un nombre"                           (pour utilisateur)
lire chiffre
calcul ← chiffre*chiffre
ecrire "resultat:", calcul                          (pour utilisateur)
fin
******************************

Exercice 2.3
Ecrire un programme qui demande son prénom à l'utilisateur, et qui lui réponde par un charmant « Bonjour » suivi du prénom. On aura ainsi le dialogue suivant :

machine : Quel est votre prénom ?
utilisateur : Marie-Cunégonde
machine : Bonjour, Marie Cunégonde ! ».


Variable prénom,  alphabétique

écrire "qu'elle est votre prénom?"
lire prénom
réponse "bonjour + prénom"
écrire "bonjour", "prénom" ,"!"


*****************************


Exercice 2.4
Ecrire un programme qui lit le prix HT d’un article, le nombre d’articles et le taux de TVA, et qui fournit le prix total TTC correspondant. Faire en sorte que des libellés apparaissent clairement.


Variable prixht, tva, prixttc,nbr en numerique

Début
écrire "saisir prix ht d'un article:"
lire prixht
écrire "saisir le nombre d’articles:"
lire nbr
écrire "saisir le taux de tva:"
lire tva
prixttc nbr*prixht *(1+tva)
écrire "le prix total TTC est:"


fin

******************************************************************************************************************************************************


                                                            PARTIE 3
                                                            Enonce des Exercices


Exercice 3.1
Ecrire un algorithme qui demande un nombre à l’utilisateur, et l’informe ensuite si ce nombre est positif ou négatif (on laisse de côté le cas où le nombre vaut zéro).

Variable nbr en numérique

écrire "saisir un nombre"
lire nbr
if nbr>0 alors 
ecrire "ce nombre est positif"
else 
écrire "ce nombre est negatif"
finsi
fin
**********************************

Exercice 3.2
Ecrire un algorithme qui demande deux nombres à l’utilisateur et l’informe ensuite si leur produit est négatif ou positif (on laisse de côté le cas où le produit est nul). Attention toutefois : on ne doit pas calculer le produit des deux nombres.

Variable nbr1, nbr2 en numerique
écrire "saisir deux nombre"
lire nbr1 et nbr2
if (nbr1>0 et nbr2>0) ou (nbr1<0 et nbr2 < 0) alors
écrire "leur produit sont positif"
else
écrire "leur produit sont negatif"
finsi
fin


********************************************************************************************************************************************************

                                                                PARTIE 4
                                                                Enonce des Exercices



                                                                 Encore un peu de logique




Exercice 4.1
Formulez un algorithme équivalent à l’algorithme suivant :

Si Tutu <= Toto + 4 OU Tata <> "OK" Alors
  Tutu ← Tutu - 1

Sinon
  Tutu ← Tutu + 1
Finsi



Exercice 4.6
Cet exercice, du pur point de vue algorithmique, n'est pas très méchant. En revanche, il représente dignement la catégorie des énoncés piégés.
En effet, rien de plus facile que d'écrire : si le candidat a plus de 50%, il est élu, sinon s'il a plus de 12,5 %, il est au deuxième tour, sinon il est éliminé. Hé hé hé... mais il ne faut pas oublier que le candidat peut très bien avoir eu 20 % mais être tout de même éliminé, tout simplement parce que l'un des autres a fait plus de 50 % et donc qu'il n'y a pas de deuxième tour !...
Moralité : ne jamais se jeter sur la programmation avant d'avoir soigneusement mené l'analyse du problème à traiter.

Variables A, B, C, D en Numérique
Variables C1, C2, C3, C4 en Booléen
Début
Ecrire "Entrez les scores des quatre candidats:"
Lire A, B, C, D
C1 ← A > 50
C2 ← B > 50 ou C > 50 ou D > 50
C3 ← A >= B et A >= C et A >= D
C4 ← A >= 12,5
Si C1 Alors
  Ecrire “Elu au premier tour"
Sinonsi C2 ou Non(C4) Alors
  Ecrire “Battu, éliminé, sorti !!!”
SinonSi C3 Alors
  Ecrire "Ballotage favorable"
Sinon
  Ecrire "Ballotage défavorable"
FinSi
Fin


*********************************************************************************************************



                                                                PARTIE 5
                                                                Les Boucles
                                                            Enonce des Exercices



Exercice 5.1
Ecrire un algorithme qui demande à l’utilisateur un nombre compris entre 1 et 3 jusqu’à ce que la réponse convienne.

Variable N en entier
Début 
écrire "saisir un nombre entre 1 et 3"
tant que n <1 ou n>3
lire n 
si n< 1 ou n>3 alors 
écrire "error recommencer"
finsi
fintantque
fin

**********************************

Exercice 5.10
Lire la suite des prix (en euros entiers et terminée par zéro) des achats d’un client. Calculer la somme qu’il doit, lire la somme qu’il paye, et simuler la remise de la monnaie en affichant les textes "10 Euros", "5 Euros" et "1 Euro" autant de fois qu’il y a de coupures de chaque sorte à rendre.

Variables E, somd, Mont, Reste, Nbr10E, Nbr5E En Entier
Debut
E ← 1
somd ← 0
TantQue E <> 0
  Ecrire "Entrez le montant : "
  Lire E
  somd ← somd + E
FinTantQue
Ecrire "Vous devez :", somd, " euros"
Ecrire "Montant versé :"
Lire Mont
Reste ← M - somd
Nbr10E ← 0
TantQue Reste >= 10
  Nbr10E ← Nbr10E + 1
  Reste ← Reste – 10
FinTantQue
Nb5E ← 0
Si Reste >= 5
  Nbr5E ← 1
  Reste ← Reste – 5
FinSi
Ecrire "Rendu de la monnaie :"
Ecrire "Billets de 10 E : ", Nbr10E
Ecrire "Billets de  5 E : ", Nbr5E
Ecrire "Pièces de 1 E : ", reste
Fin

*************************************************************************************************************************************
                                                PARTIE 6
                                                Les Tableaux
                                            Enonce des Exercices





Exercice 6.1
Ecrire un algorithme qui déclare et remplisse un tableau de 7 valeurs numériques en les mettant toutes à zéro.
tableau val (7)
variable i en numérique
pour i ← 0 à 7
val(i) ← 0
i suivant
fin


*************************************************************************************************************************************

                                                    Partie 7
                                                    Techniques Rusees




Exercice 7.1

Variables Nb, i en Entier
Variable Flag en Booleen
Tableau T() en Entier
Debut
Ecrire "Entrez le nombre de valeurs :"
Lire Nb
Redim T(Nb-1)
Pour i ← 0 à Nb - 1
  Ecrire "Entrez le nombre n° ", i + 1
  Lire T(i)
i Suivant
Flag ← Vrai
Pour i ← 1 à Nb - 1
  Si T(i) <> T(i – 1) + 1 Alors
    Flag ← Faux
  FinSi
i Suivant
Si Flag Alors
  Ecrire "Les nombres sont consécutifs"
Sinon
  Ecrire "Les nombres ne sont pas consécutifs"
FinSi
Fin
Cette programmation est sans doute la plus spontanée, mais elle présente le défaut d'examiner la totalité du tableau, même lorsqu'on découvre dès le départ deux éléments non consécutifs. Aussi, dans le cas d'un grand tableau, est-elle dispendieuse en temps de traitement. Une autre manière de procéder serait de sortir de la boucle dès que deux éléments non consécutifs sont détectés. La deuxième partie de l'algorithme deviendrait donc :
i ← 1
TantQue T(i) = T(i – 1) + 1 et i < Nb - 1
  i ← i + 1
FinTantQue
Si T(i) = T(i – 1) + 1 Alors
  Ecrire "Les nombres sont consécutifs"
Sinon
  Ecrire "Les nombres ne sont pas consécutifs"
FinSi
*************************************************

Exercice 7.2
Ecrivez un algorithme qui trie un tableau dans l’ordre décroissant.
Vous écrirez bien entendu deux versions de cet algorithme, l'une employant le tri par sélection, l'autre le tri à bulles.

Trie par selection
variable N entier

pour i ← 0 à N - 2
posmax = i
pour j ← i + 1 à N
si t(j) > t(posmaxi) alors 
posmax ← j
finsi 
j suivant
  temp ← t(posmaxi)
  t(posmaxi) ← t(i)
  t(i) ← temp
i suivant
Fin

Tri à bulles :

Variable Yapermute en Booléen
Début
TantQue Yapermute
pour i ← 0 à N - 2
Si t(i) < t(i+1) alors
temps ← t(i)
t(i) ← t(i+1)
t(i-1) ← temp
    Yapermut ← Vrai
    Finsi
  i suivant
FinTantQue
Fin


*************************************************************************************************************************************
                                                        Partie 9
                                                        Les Fonctions Prédéfinies



Exercice 9.1
Parmi ces affectations (considérées indépendamment les unes des autres), lesquelles provoqueront des erreurs, et pourquoi ?

Variables A, B, C en Numérique
Variable D en Caractère
A ← Sin(B)                  ok pas de problème
A ← Sin(A + B * C)          ok pas de problème
B ← Sin(A) – Sin(D)         erreur car valeur de D en caractère
C ← Sin(A / B)              ok pas de problème à part si B égale 0
C ← Cos(Sin(A)              erreur car manque une parenthèse après (A)

***************************

Exercice 9.11
Ecrivez les algorithmes qui génèrent un nombre Glup aléatoire tel que …
0 =< Glup < 2
–1 =< Glup < 1
1,35 =< Glup < 1,65
Glup émule un dé à six faces
–10,5 =< Glup < +6,5
Glup émule la somme du jet simultané de deux dés à six faces

a) Glup ← Alea() * 2
b) Glup ← Alea() * 2 - 1
c) Glup ← Alea() * 0,30 + 1,35
d) Glup ← Ent(Alea() * 6) + 1
e) Glup ← Alea() * 17 – 10,5
f) Glup ← Ent(Alea()*6) + Ent(Alea()*6) + 2


******************************************************************************************************************************

                                                            PARTIE 10
                                                            Enoncé des Exercices


Exercice 10.1
Quel résultat cet algorithme produit-il ?

Variable Truc en Caractère
Début
Ouvrir "Exemple.txt" sur 5 en Lecture
Tantque Non EOF(5)
  LireFichier 5, Truc
  Ecrire Truc
FinTantQue
Fermer 5
Fin

résultat : "Exemple.txt"

*********************************************************************************************************************************

                                                            Partie 11
                                                            Procédures et Fonctions


Exercice 11.1
Écrivez une fonction qui renvoie la somme de cinq nombres fournis en argument.

fonction sum(1+2+3+4+5+6)en numerique
renvoyer 1+2+3+4+5+6
fin fonction






