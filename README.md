
L'objectif de ce projet et de prédire l'evolution mensuelle des passagers d'une compagnie aérienne

Pour se faire on dispose d'une Série  brute airpass : nombre mensuel de passagers aériens, en milliers, de janvier 1949 à décembre 1960.


1ere étape :Analyse de la série

    apres analyse de la serie celle ci montre une tendance croissante et des saisonnalités se produisant chaque année (donc de période 12)


Etape2 :
    les saisonnalités ne permettant pas de comparer des instants consécutifs de la série il faut donc la corriger de ces valeurs saisonnieres avant de pouvoir faire des prévisions


Etape 3 :test de différents modèle  pour la prévision:

    correction des valeurs saisonnieres:
        methode des moyennes mobile pour la correction des valeur saisonnieres

    prévisions:
        lissage exponnetiel simple : pas satisfaisant car prevision connstante
        lissage exponentiel double: pas satisfaisant car prevision lineaire suivant la tendance

        modele Sarima: la série n'etant pas stationnaire il a fallu la stationnarisé (voir notebook)
            model efficace avec rmse=18.59 et mape=2.90
