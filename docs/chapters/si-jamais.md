<!-- .slide: class="chapter" -->
## 5
### Les autres choses éventuellement utiles





<!-- .slide: class="slide" -->
### Paramétrage des variables de sortie






<!-- .slide: class="slide" -->
### Pagination des résultats
Les résultats affichent par défaut au plus les 20 premiers unités légales ou établissements.
Il est possible de paramétrer cela par des paramètres : 
- **nombre** : nombre d'unités légales ou établissements par page (entre 0 et 100 000)
- **debut** : rang du premier élément de la page (par défaut 0, limité à 1 000 000) 
```
/ws/siren?nombre=3&debut=10
```
Pour parcourir de manière plus efficace, il existe des curseurs.
```
/ws/siren?curseur=*
```
Le retour et l'en-tête Link contiennent alors le curseur suivant à pointer
```
/ws/siren?curseur=AoEpMDA1NDEwNzU4
```





<!-- .slide: class="slide" -->
### Les facettes
Elles servent à effectuer des comptages par catégorie
**Syntaxe** : facette.champ=champ1,champ2...







