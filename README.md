# Template API Rails  

### 1. Générer l'API avec la commande suivante :  

``` 
$ rails new NomDeVotreApp --api -m ../chemin/vers/le/fichier/template.rb
```

Ceci va créer une nouvelle application Rails API  
(Comparé  à une application Rails standard, elle est allégée de certaines parties inutiles pour une API. Ainsi, par exemple, les views ne seront pas générées automatiquement).

De plus, ce template installe et configure :
- Devise
- Devise-JWT
- Les routes Signup, Login, etc..
- Un namespace /api/
- Rspec ainsi qu'une série de tests
- Toutes les gems utiles
- ...etc

### 2. Vérifier que tout fonctionne  

Les tests sont déjà codés, donc il ne reste plus qu'à exécuter la commande suivante :

```
$ foreman run rake
```

### 3. Utiliser l'API
L'authentification se fait avec le token JWT depuis le header 'Authorization'. Voir spec/controllers/user_controller_spec.rb pour avoir un exemple.

Ce token sera généré lors du signup ou d'un login et retourné dans le header de la réponse.

### Enjoy ! :wink:

***********************
Template original initialement forked depuis :  
https://github.com/jameschambers/boring-bits-rails-api  
Quelques corrections ont été apportées