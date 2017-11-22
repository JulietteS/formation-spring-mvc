<!-- .slide: class="chapter" -->
## 5
### Les autres choses éventuellement utiles





<!-- .slide: class="slide" -->
### Paramétrage des variables de sortie
Pour rendre les retours moins bavards, on peut limiter les variables sur le principe d'une liste blanche
```
/ws/siren?champs=Prenom1,Prenom2
```





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
**Syntaxe** : facette.champ=champ1, champ2...
```
/ws/siret?q=periode(EtatAdministratifEtablissement:A) AND CodeCommuneEtablissement:75*&date=2018-01-01&nombre=0&facette.champ=ActivitePrincipale
```
```json
{
    "Header": {
        "Statut": 200,
        "Message": "ok",
        "Total": 861090,
        "Debut": 0,
        "Nombre": 0
    },
    "Etablissements": [],
    "Facettes": [
        {
            "Nom": "ActivitePrincipale",
            "Comptages": [
                {
                    "Valeur": "68.20B",
                    "Nombre": 101470
                },
                {
                    "Valeur": "70.22Z",
                    "Nombre": 49949
                },
                {
                    "Valeur": "81.10Z",
                    "Nombre": 41581
                },
                {
                    "Valeur": "94.99Z",
                    "Nombre": 36072
                },
                {
                    "Valeur": "68.20A",
                    "Nombre": 32765
                },
                {
                    "Valeur": "69.10Z",
                    "Nombre": 32178
                },
                {
                    "Valeur": "90.01Z",
                    "Nombre": 19229
                },
                {
                    "Valeur": "90.03A",
                    "Nombre": 18993
                },
                {
                    "Valeur": "64.20Z",
                    "Nombre": 17385
                },
                {
                    "Valeur": "56.10A",
                    "Nombre": 15053
                }
            ]
        }
    ]
}
```
...et beaucoup plus de possibilités sur les facettes (voir la documentation officielle)


