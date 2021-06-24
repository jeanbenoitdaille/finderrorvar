# finderrorvar
Trouver l'erreur : variable égale à zéro 
Dans ce cas-ci, on veut vérifier que la variable a contient bien un nombre.

Pour rapidement vérifier qu'une variable contient des données, on peut utiliser une structure conditionnelle de base.

Par exemple pour vérifier qu'une liste n'est pas vide, on peut faire :

    ma_liste = [1, 2, 3]
    if ma_liste:
        print("La liste n'est pas vide")

Au lieu de :

    ma_liste = [1, 2, 3]
    if len(ma_liste) > 0:
        print("La liste n'est pas vide")

Vous conviendrez que la première façon de faire est plus concise est lisible. Cependant, en prenant l'habitude de cette syntaxe, on peut tomber dans l'écueil qu'il fallait résoudre dans cet exercice.

En effet, imaginons qu'à la place d'une liste, nous récupérons cette fois-ci un nombre entier. Si le nombre récupéré est 0, alors la structure conditionnelle ne sera pas vérifiée, car 0 est équivalant à False.

C'est pourquoi dans ce cas-ci, nous ne pouvons pas utiliser la syntaxe simplifiée if variable, il faut donc vérifier explicitement que la variable n'est pas égale à None :

    a = 0
    if a is not None:
        print("La variable n'est pas égale à None")
