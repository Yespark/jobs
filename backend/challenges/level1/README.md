# Yespark Backend Challenge

Looking for a job? Check out our [open positions](https://www.yespark.fr/jobs)

## A propos de Yespark

Yespark est le leader en France de la locaction de parking au mois. Notre backend est construit sur le framework web [Ruby on Rails](http://rubyonrails.org/). Nous utilisons la plate-forme de service [Heroku](https://dashboard.heroku.com/) pour mettre en ligne notre API et notre [application web](https://www.yespark.fr). Notre réseau de parkings en location compte environ 300 parkings dans toute la France. Notre force ? Un service client de qualité, des applications smartphones [iOS](https://itunes.apple.com/fr/app/yespark/id891832557?mt=8) et [Android](https://play.google.com/store/apps/details?id=com.yespark.android&hl=fr) à la pointe des technologies mobiles natives, une équipe jeune et dynamique. Cela nous permet de proposer des parkings en location environ 30% moins chers que les locations traditionnelles.

## Challenge n°1

### Créer une application web sur Heroku qui permette de créer, modifier et supprimer des objets `Parking`.

On se donne comme entrée le fichier `input.json`, l'objectif est de créer le fichier `output.json`.
Les attributs qui diffèrent entre le fichier d'entrée et de sortir sont :
- `id`, de type `integer`, qui représente l'identifiant du parking dans la base de données ;
- `lat` et `lng`, de type `float`, qui représentent les coordonéees du parking. Il s'agit donc de trouver ces coordonnées à partir de l'adresse du parking. On pourra notamment s'appuyer sur la gem [Geokit](https://github.com/geokit/geokit) ;
- `slug`, de type `string`, qui représente un label court, qui identifie de manière unique un parking ;
- `district`, de type `string`, qui représente l'arrondissement, différent de `"0"` si la ville est Paris.

L'application web prendra la forme d'une interface administrateur (backoffice dans le jargon) qui contient les pages suivantes :
- la page d'accueil, avec un tableau de tous les parkings et leurs attributs, et la possibilité de créer ou de supprimer un parking ;
- une page d'édition d'un parking, avec la possibilité de modifier ses attributs ;
- une page enfin qui affiche une carte Google Maps de la France, avec un marquer pour chaque parking.

Pour information, la création d'une application web sur la plate-forme Heroku prend moins de 5 minutes, comme l'explique cette [vidéo](https://vimeo.com/6916740) (vimeo).