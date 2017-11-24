<!-- .slide: class="chapter" -->
## 4
### Recherche avancée





<!-- .slide: class="slide" -->
### Recherche phonétique
Il est possible de faire des recherches phonétiques sur la dénomination, à la fois au niveau des unités légales (yc l'historique de dénomination) et au niveau des établissements. L'algorithme utilisé (*Beider-Morse*) génère assez peu de faux positifs (comparé à *Daitch-Mokotoff Soundex*)

 1. À partir du mot saisi, il essaie de deviner la langue (environ 200 règles) parmi 15
 2. avec cette langue, il effectue une transcription phonétique d'abord exacte puis approchée
 3. s'il n'arrive pas à déduire une langue, il fait une transcription phonétique générique exacte puis approchée
 4. il recherche les échos correspondants dans l'index





<!-- .slide: class="slide" -->
### Recherche phonétique : exemple 1
```
/ws/siret?q=DenomPhon:Jairome&champs=Denomination&nombre=3
```
```json
{
    "Header": {
        "Statut": 200,
        "Message": "ok",
        "Total": 7248,
        "Debut": 0,
        "Nombre": 3
    },
    "Etablissements": [
        {
            "UniteLegale": {
                "Denomination": "JEROME ET CHENAUD EPSE JEROME"
            }
        },
        {
            "UniteLegale": {
                "Denomination": "JEROME"
            }
        },
        {
            "UniteLegale": {
                "Denomination": "JEROME"
            }
        }
    ]
}
```





<!-- .slide: class="slide" -->
### Recherche phonétique : exemple 2
```
/ws/siret?q=Denomination:Stehle&champs=Denomination&nombre=1
```
```json
{
    "Header": {
        "Statut": 200,
        "Message": "ok",
        "Total": 12,
        "Debut": 0,
        "Nombre": 1
    },
    "Etablissements": [
        {
            "UniteLegale": {
                "Denomination": "SCI STEHLE"
            }
        }
    ]
}
```
```
/ws/siret?q=DenomPhon:Stehle&champs=Denomination&nombre=1
```
```json
{
    "Header": {
        "Statut": 200,
        "Message": "ok",
        "Total": 5537,
        "Debut": 0,
        "Nombre": 1
    },
    "Etablissements": [
        {
            "UniteLegale": {
                "Denomination": "STELI"
            }
        }
    ]
}
```





<!-- .slide: class="slide" -->
### La pondération et le score
Le moteur de recherche calcule un score pour chaque requête et chaque document. Le score est fonction de :
 * la fréquence du terme dans les champs demandés du document $tf(t \in d)$
 * la fréquence inverse du terme dans tous les documents $idf(t)$
 * le boost du terme $t.getBoost()$
 * la normalisation du champ $norm(t,d)$
 * un facteur de coordination (nombre de termes de la recherche dans le document/nombre de termes dans la recherche) $coord(q,d)$
 * une normalisation de requête $queryNorm(q)$


$Score(q,d) = \sum_{t \in q} \left\( tf(t \in d) \cdot idf(t)^2 \cdot t.getBoost() \cdot norm(t,d) \right\) \cdot coord(q,d) \cdot queryNorm(q)$






<!-- .slide: class="slide" -->
### La pondération et le score
La pondération permet de modifier le poids d'un champ dans une requête multicritère

**Syntaxe** : ponderation(nomVariable1\*ponderation1 nomVariable2\*ponderation2:valeur) 

```
/ws/siret?q=ponderation(Denomination*1.5 DenomPhon:Stehle)&champs=Denomination,Score&nombre=3
```

```json
{
    "Header": {
        "Statut": 200,
        "Message": "ok",
        "Total": 5537,
        "Debut": 0,
        "Nombre": 3
    },
    "Etablissements": [
        {
            "Score": 21.902185,
            "UniteLegale": {
                "Denomination": "SCI STEHLE"
            }
        },
        {
            "Score": 17.408476,
            "UniteLegale": {
                "Denomination": "JEAN LUC STEHLE CONSEIL"
            }
        },
        {
            "Score": 17.408476,
            "UniteLegale": {
                "Denomination": "SOCIETE STEHLE GMBH"
            }
        }
    ]
}
```
