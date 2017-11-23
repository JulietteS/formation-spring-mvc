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
/ws/siret?q=Denomination:Stehle&champs=Denomination&nombre=3
```
```json
{
    "Header": {
        "Statut": 200,
        "Message": "ok",
        "Total": 12,
        "Debut": 0,
        "Nombre": 3
    },
    "Etablissements": [
        {
            "UniteLegale": {
                "Denomination": "SCI STEHLE"
            }
        },
        {
            "UniteLegale": {
                "Denomination": "JEAN LUC STEHLE CONSEIL"
            }
        },
        {
            "UniteLegale": {
                "Denomination": "SOCIETE STEHLE GMBH"
            }
        }
    ]
}
```
```
/ws/siret?q=DenomPhon:Stehle&champs=Denomination&nombre=10
```
```json
{
    "Header": {
        "Statut": 200,
        "Message": "ok",
        "Total": 5537,
        "Debut": 0,
        "Nombre": 10
    },
    "Etablissements": [
        {
            "UniteLegale": {
                "Denomination": "STELI"
            }
        },
        {
            "UniteLegale": {
                "Denomination": "STELEA"
            }
        },
        {
            "UniteLegale": {
                "Denomination": "STELIE"
            }
        },
        {
            "UniteLegale": {
                "Denomination": "STELIE"
            }
        },
        {
            "UniteLegale": {
                "Denomination": "STELI"
            }
        },
        {
            "UniteLegale": {
                "Denomination": "STELI"
            }
        },
        {
            "UniteLegale": {
                "Denomination": "STELI"
            }
        },
        {
            "UniteLegale": {
                "Denomination": "STELI"
            }
        },
        {
            "UniteLegale": {
                "Denomination": "STELOY"
            }
        },
        {
            "UniteLegale": {
                "Denomination": "STELI"
            }
        }
    ]
}
```





<!-- .slide: class="slide" -->
### La pondération
