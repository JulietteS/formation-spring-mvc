<!-- .slide: data-background-image="images/spring.png" data-background-size="1200px" class="chapter" -->
## 2
### Recherche sur les établissements





<!-- .slide: class="slide" -->
<h3>Présentation du service</h3>
Obtenir les informations du répertoire sur un établissement, identifiée par son <span style="color:red">siret</span>
 - l'historique complet (sur enseigne, activité principale de l'établissement, état, caractère employeur)
 - l'état à une date donnée
 - l'état courant (à la date de la base)





<!-- .slide: class="slide" -->
### Appel au service

GET /ws/siret/{siret}
GET /ws/siret/{siret}?date={date}

| Paramètre               | Description | Type de paramètre | Type  | Obligatoire                              |
| ----------------------- | ------------|-------------------|-------|----------------------------------------- |
| `siret`                 | Numéro siret de l'établissement (14 chiffres) | Path | String | Oui 												       |
| `date`                  | Date à laquelle on souhaite connaître l'état (AAAA-MM-JJ) | Query | String | Non   |
| `Accept`                | Format de la réponse demandé (par défaut Application/json), demander Text/csv pour du CSV |Header|String| Non |





<!-- .slide: class="slide" -->
### Exemple de requête sur le siret

GET /ws/siret/39860733300059

```json
{
    "Header": {
        "Statut": 200,
        "Message": "ok"
    },
    "Etablissement": {
        "Siren": "398607333",
        "Nic": "00059",
        "StatutDiffusionEtablissement": "O",
        "DateCreationEtablissement": "2015-01-09",
        "NombrePeriodes": 4,
        "UniteLegale": {
            "StatutDiffusionUniteLegale": "O",
            "DateCreationUniteLegale": "1994-10-10",
            "Sigle": null,
            "Sexe": 1,
            "NomUsage": null,
            "Prenom1": "BERTRAND",
            "Prenom2": "CHARLES",
            "Prenom3": null,
            "Prenom4": null,
            "PrenomUsuel": "BERTRAND",
            "CaractereEmployeur": "O",
            "EtatAdministratif": "A",
            "Nom": "GRONDIN",
            "Denomination": null,
            "ActivitePrincipale": "47.81Z",
            "LibelleActivite": "Commerce de détail alimentaire sur éventaires et marchés",
            "NomenclatureActivite": "NAFRev2",
            "CategorieJuridique": null,
            "CategorieProfessionnelle": "1000",
            "NICSiege": "00075"
        },
        "Adresse": {
            "ComplementAdresseEtablissement": null,
            "NumeroVoieEtablissement": "44",
            "IndiceRepetitionEtablissement": null,
            "TypeVoieEtablissement": "RUE",
            "LibelleVoieEtablissement": "NANTIER DIDIEE",
            "CodePostalEtablissement": "97490",
            "LibelleCommuneEtablissement": "SAINT DENIS",
            "LibelleCommuneEtrangerEtablissement": null,
            "DistributionSpecialeEtablissement": null,
            "CodeCommuneEtablissement": "97411",
            "CedexEtablissement": null
        },
        "Periodes": [
            {
                "DateFin": null,
                "DateDebut": "2016-04-01",
                "EtatAdministratifEtablissement": "F",
                "IndEtatAdministratifEtablissement": true,
                "ActivitePrincipaleEtablissement": "56.10C",
                "LibelleActiviteEtablissement": "Restauration de type rapide",
                "NomenclatureActiviteEtablissement": "NAFRev2",
                "IndActivitePrincipaleEtablissement": false,
                "CaractereEmployeurEtablissement": "N",
                "IndCaractereEmployeurEtablissement": false,
                "Enseigne1": "MON CHINOIS PREFERE",
                "Enseigne2": null,
                "Enseigne3": null,
                "IndEnseigneEtablissement": false
            },
            {
                "DateFin": "2016-03-31",
                "DateDebut": "2016-02-16",
                "EtatAdministratifEtablissement": "A",
                "IndEtatAdministratifEtablissement": false,
                "ActivitePrincipaleEtablissement": "56.10C",
                "LibelleActiviteEtablissement": "Restauration de type rapide",
                "NomenclatureActiviteEtablissement": "NAFRev2",
                "IndActivitePrincipaleEtablissement": true,
                "CaractereEmployeurEtablissement": "N",
                "IndCaractereEmployeurEtablissement": false,
                "Enseigne1": "MON CHINOIS PREFERE",
                "Enseigne2": null,
                "Enseigne3": null,
                "IndEnseigneEtablissement": true
            },
            {
                "DateFin": "2016-02-15",
                "DateDebut": "2015-04-27",
                "EtatAdministratifEtablissement": "A",
                "IndEtatAdministratifEtablissement": false,
                "ActivitePrincipaleEtablissement": "47.81Z",
                "LibelleActiviteEtablissement": "Commerce de détail alimentaire sur éventaires et marchés",
                "NomenclatureActiviteEtablissement": "NAFRev2",
                "IndActivitePrincipaleEtablissement": false,
                "CaractereEmployeurEtablissement": "N",
                "IndCaractereEmployeurEtablissement": true,
                "Enseigne1": "CHAPO LA PAILLE",
                "Enseigne2": null,
                "Enseigne3": null,
                "IndEnseigneEtablissement": false
            },
            {
                "DateFin": "2015-04-26",
                "DateDebut": "2015-01-09",
                "EtatAdministratifEtablissement": "A",
                "IndEtatAdministratifEtablissement": true,
                "ActivitePrincipaleEtablissement": "47.81Z",
                "LibelleActiviteEtablissement": "Commerce de détail alimentaire sur éventaires et marchés",
                "NomenclatureActiviteEtablissement": "NAFRev2",
                "IndActivitePrincipaleEtablissement": true,
                "CaractereEmployeurEtablissement": "O",
                "IndCaractereEmployeurEtablissement": true,
                "Enseigne1": "CHAPO LA PAILLE",
                "Enseigne2": null,
                "Enseigne3": null,
                "IndEnseigneEtablissement": true
            }
        ]
    }
}
```





<!-- .slide: class="slide" -->
### Exemple de requête sur le siret (2)

GET /ws/siret/39860733300059?date=2018-01-01

Période courante

```json
{
    "Header": {
        "Statut": 200,
        "Message": "ok"
    },
    "Etablissement": {
        "Siren": "398607333",
        "Nic": "00059",
        "StatutDiffusionEtablissement": "O",
        "DateCreationEtablissement": "2015-01-09",
        "NombrePeriodes": 4,
        "UniteLegale": {
            "StatutDiffusionUniteLegale": "O",
            "DateCreationUniteLegale": "1994-10-10",
            "Sigle": null,
            "Sexe": 1,
            "NomUsage": null,
            "Prenom1": "BERTRAND",
            "Prenom2": "CHARLES",
            "Prenom3": null,
            "Prenom4": null,
            "PrenomUsuel": "BERTRAND",
            "CaractereEmployeur": "O",
            "EtatAdministratif": "A",
            "Nom": "GRONDIN",
            "Denomination": null,
            "ActivitePrincipale": "47.81Z",
            "LibelleActivite": "Commerce de détail alimentaire sur éventaires et marchés",
            "NomenclatureActivite": "NAFRev2",
            "CategorieJuridique": null,
            "CategorieProfessionnelle": "1000",
            "NICSiege": "00075"
        },
        "Adresse": {
            "ComplementAdresseEtablissement": null,
            "NumeroVoieEtablissement": "44",
            "IndiceRepetitionEtablissement": null,
            "TypeVoieEtablissement": "RUE",
            "LibelleVoieEtablissement": "NANTIER DIDIEE",
            "CodePostalEtablissement": "97490",
            "LibelleCommuneEtablissement": "SAINT DENIS",
            "LibelleCommuneEtrangerEtablissement": null,
            "DistributionSpecialeEtablissement": null,
            "CodeCommuneEtablissement": "97411",
            "CedexEtablissement": null
        },
        "Periodes": [
            {
                "DateFin": null,
                "DateDebut": "2016-04-01",
                "EtatAdministratifEtablissement": "F",
                "IndEtatAdministratifEtablissement": true,
                "ActivitePrincipaleEtablissement": "56.10C",
                "LibelleActiviteEtablissement": "Restauration de type rapide",
                "NomenclatureActiviteEtablissement": "NAFRev2",
                "IndActivitePrincipaleEtablissement": false,
                "CaractereEmployeurEtablissement": "N",
                "IndCaractereEmployeurEtablissement": false,
                "Enseigne1": "MON CHINOIS PREFERE",
                "Enseigne2": null,
                "Enseigne3": null,
                "IndEnseigneEtablissement": false
            }
        ]
    }
}
```
