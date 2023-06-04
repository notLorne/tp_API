# tp_API

À remettre le 13 juin 2023 avant 23h59 | Équipe de 2 (30%)
TP1 : Rapide & Dangereux (Édition ville de Montréal)

Introduction

Vous devez construire votre propre RestAPI qui fournira des informations supplémentaires
pertinentes aux utilisateurs de votre système à partir de celui offert par la ville de Montréal
(https://donnees.montreal.ca/dataset/collisions-routieres). Ce qui vous distinguera de vos
concurrents est la pertinence des données fournies. Voici la liste des fonctionnalités requises :


Cas 1 : Récupérer/Convertir les données (20 points)
D’abord, il faut pouvoir récupérer les données de l’API de la ville de Montréal et de les afficher
de la méthode que vous voulez. Ensuite, assurez-vous que si l’API de la ville n’est pas disponible,
que vous soyez en mesure de convertir les données du CSV fourni sur leur site en JSON afin de
les afficher, encore une fois, de la méthode que vous voulez.


Cas 2 : Insérer les données dans MongoDB (20 points)
Il s’agit d’insérer le contenu que vous récupérer dans votre base de données. On doit pouvoir y
retrouver toutes les informations reçues par l’API ou le fichier CSV.


Cas 3 : Gérer les données obsolètes (20 points)
Il s’agit ici d’implémenter une mécanique de « cache ». Lorsque l’on fait appel à votre API, il faut
faire en sorte de retourner des données récentes. Dans certains APIs, on a une limite sur le
nombre de fois que l’on peut l’interroger. Même si ce n’est pas le cas ici, trouvez une manière de
de minimiser les appels vers l’API de la ville de Montréal. Une donnée est considérée récente si
elle a moins d’une journée (24h) depuis le dernier appel à l’API externe de la ville.


Cas 4 : Visualiser les données (20 points)
Il faut pouvoir visualiser les données qui nous intéresse. On n’affichera pas tous les éléments
contenus dans notre base de données. Il faut donc afficher uniquement 10 informations au
total. Affichez les 5 données descriptives que vous trouvez les plus pertinentes et affichez 5
métriques d’agrégations (statistiques) représentant des faits saillants. Par exemple, l’année où il
y a eu le moins de mort. Présentez les résultats sous formes de deux tableaux.


Cas 5 : Ajouter un repère « marker » sur une carte (20 points)
Il faut utiliser l’API de Google (Maps) ou un autre de votre choix. Vous devrez effectuer vos
recherches et lire la documentation pour savoir comment l’utiliser. Choisissez la métrique du cas
4 que vous trouvez la plus intéressante et afficher un repère sur ce lieu. Par exemple, affichez un
repère à l’endroit où il y a eu le maximum de morts
