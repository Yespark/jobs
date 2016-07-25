# Yespark Backend Challenge

Looking for a job? Check out our [open positions](https://www.yespark.fr/jobs)

## Connais-tu Yespark, le leader de la location de parking au mois ?

1. A partir des informations disponibles sur [internet](https://www.yespark.fr/) et les applications ([iOS](https://itunes.apple.com/fr/app/yespark/id891832557?mt=8) et [Android](https://play.google.com/store/apps/details?id=com.yespark.android&hl=fr)), schématise la base de données que nous utilisons. L'objectif est de trouver le maximum de tables et de relations, pas de trouver le maximum d'attributs.

2. L'administrateur supprime l'utilisateur dont l'identifiant est 12. Que donnent respectivement les requêtes `User.find(12)` et `User.find_by_id(12)` ?

3. Quelles sont tes gems Ruby préférées, et pourquoi ?

4. En règle générale, en Ruby, vaut-il mieux écrire une fonction itérative ou récursive, et pourquoi ?

5. Qu'est-ce que Rails ? Rack middleware ? L'asset pipeline ?

6. Qu'est-ce qui distingue les closures Lambda, Blocks et Proc ? Une classe et un module ?

7. Quelles routes seront construites avec le code suivant :

```ruby
resources :parkings do
  member do
    get 'reviews'
  end
  collection do
    post 'bulk_import'
  end
end
```

8. Donne une définition de l'architecture MVC de Ruby on Rails. Tu peux t'appuyer sur l'exemple de [l'affichage de la page d'un parking](https://www.yespark.fr/parkings/montgallet).
