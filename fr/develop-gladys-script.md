##Développer un script

<div class="alert alert-info" role="alert" style="padding: 10px;">Attention, cette documentation s'adresse à la version 3.0 de Gladys. La version 2 étant bientôt deprecated, inutile de développer pour la v2 !</div>

Les script dans Gladys vous permettent de créer des petits programmes en javascript, afin de faire des actions beaucoup plus fines qu'avec un scénario.

### Sandbox

Les scripts tournent dans une sandbox, ils n'ont volontairement pas accès à toute l'API de Node.js. Vous ne pouvez par exemple pas faire de `require` dans un script.

### Les fonctions disponibles

Vous pouvez faire appel à toutes les fonctions de l'API de Gladys ( voir la catégorie suivante de la documentation ), et à toutes les fonctions des modules.

Les fonctions des modules sont accessible sous l'objet :

```javascript
gladys.modules.NOM_MODULE
```

Si le module `test` a une fonction `getWeather()`, on peut faire :

```javascript
gladys.modules.test.getWeather();
```