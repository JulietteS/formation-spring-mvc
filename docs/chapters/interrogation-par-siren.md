<!-- .slide: class="chapter" -->
## 1
### Recherche sur les unités légales





<!-- .slide: class="slide" -->
<h3>Présentation du service</h3>
Obtenir les informations du répertoire sur une unité légale, identifiée par son <span style="color:red">siren</span>
 - l'historique complet (sur dénomination, nom de naissance, catégorie juridique, état, nic du siège, activité principale)
 - l'état à une date donnée
 - l'état courant (à la date de la base)





<!-- .slide: class="slide" -->
### Appel au service

GET /ws/siren/{siren}
GET /ws/siren/{siren}?date={date}

| Paramètre               | Description | Type de paramètre | Type  | Obligatoire                              |
| ----------------------- | ------------|-------------------|-------|----------------------------------------- |
| `siren`                 | Numéro siren de l'entreprise (9 chiffres) | Path | String | Oui 												       |
| `date`                  | Date à laquelle on souhaite connaître l'état (AAAA-MM-JJ) | Query | String | Non   |
| `Accept`                | Format de la réponse demandé (par défaut Application/json), demander Text/csv pour du CSV |Header|String| Non |





<!-- .slide: class="slide" -->
### Codes retour

| Code HTTP      | Résumé         | Raison                               |
| -------------- | ---------------|------------------------------------- |
| `200`          | OK             | Entreprise trouvée |
| `400`          | Bad Request    | Paramètres incorrects ou manquants |
| `401`          | Unauthorized   | Tentative de connection avec une adresse IP non autorisée |
| `403`          | Forbidden      | Droits insuffisants pour accéder à cette unité |
| `404`          | Not Found      | Unité non trouvée (siren inexistant ou pas encore créé à la date demandée) |
| `406`          | Not acceptable | Format demandé non prévu |
| `500`          | Internal Server Error | Ca se passe mal pour le serveur |
| `503`          | Service Unvailable | Ca se passe *très* mal pour le serveur |





<!-- .slide: class="slide" -->
### Exemple de requête sur le siren

GET /ws/siren/005520135

```json
{
    "Header": {
        "Statut": 200,
        "Message": "ok"
    },
    "UniteLegale": {
        "Siren": "005520135",
        "StatutDiffusionUniteLegale": "O",
        "DateCreationUniteLegale": "1955-01-01",
        "Sigle": null,
        "Sexe": null,
        "NomUsage": null,
        "Prenom1": null,
        "Prenom2": null,
        "Prenom3": null,
        "Prenom4": null,
        "PrenomUsuel": null,
        "CaractereEmployeur": "O",
        "TrancheEffectifsUniteLegale": "NN",
        "AnneeEffectifsUniteLegale": null,
        "NombrePeriodes": 6,
        "Periodes": [
            {
                "DateFin": null,
                "DateDebut": "2007-11-19",
                "EtatAdministratif": "C",
                "IndEtatAdministratif": true,
                "Nom": null,
                "Denomination": "CHANVI GESTION",
                "IndDesignation": false,
                "ActivitePrincipale": "74.1J",
                "LibelleActivite": "Administration d'entreprises",
                "NomenclatureActivite": "NAFRev1",
                "IndActivitePrincipale": false,
                "CategorieJuridique": "5710",
                "IndCategorieJuridique": false,
                "CategorieProfessionnelle": null,
                "IndCategorieProfessionnelle": false,
                "NICSiege": "00038",
                "IndNICSiege": false
            },
            {
                "DateFin": "2007-11-18",
                "DateDebut": "2007-04-20",
                "EtatAdministratif": "A",
                "IndEtatAdministratif": false,
                "Nom": null,
                "Denomination": "CHANVI GESTION",
                "IndDesignation": false,
                "ActivitePrincipale": "74.1J",
                "LibelleActivite": "Administration d'entreprises",
                "NomenclatureActivite": "NAFRev1",
                "IndActivitePrincipale": false,
                "CategorieJuridique": "5710",
                "IndCategorieJuridique": false,
                "CategorieProfessionnelle": null,
                "IndCategorieProfessionnelle": false,
                "NICSiege": "00038",
                "IndNICSiege": true
            },
            {
                "DateFin": "2007-04-19",
                "DateDebut": "2002-12-25",
                "EtatAdministratif": "A",
                "IndEtatAdministratif": false,
                "Nom": null,
                "Denomination": "CHANVI GESTION",
                "IndDesignation": false,
                "ActivitePrincipale": "74.1J",
                "LibelleActivite": "Administration d'entreprises",
                "NomenclatureActivite": "NAF1993",
                "IndActivitePrincipale": false,
                "CategorieJuridique": "5710",
                "IndCategorieJuridique": true,
                "CategorieProfessionnelle": null,
                "IndCategorieProfessionnelle": false,
                "NICSiege": "00020",
                "IndNICSiege": false
            },
            {
                "DateFin": "2002-12-24",
                "DateDebut": "1995-12-25",
                "EtatAdministratif": "A",
                "IndEtatAdministratif": false,
                "Nom": null,
                "Denomination": "CHANVI GESTION",
                "IndDesignation": false,
                "ActivitePrincipale": "74.1J",
                "LibelleActivite": "Administration d'entreprises",
                "NomenclatureActivite": "NAF1993",
                "IndActivitePrincipale": true,
                "CategorieJuridique": "5599",
                "IndCategorieJuridique": false,
                "CategorieProfessionnelle": null,
                "IndCategorieProfessionnelle": false,
                "NICSiege": "00020",
                "IndNICSiege": false
            },
            {
                "DateFin": "1995-12-24",
                "DateDebut": "1992-01-01",
                "EtatAdministratif": "A",
                "IndEtatAdministratif": false,
                "Nom": null,
                "Denomination": "CHANVI GESTION",
                "IndDesignation": true,
                "ActivitePrincipale": null,
                "LibelleActivite": null,
                "NomenclatureActivite": null,
                "IndActivitePrincipale": false,
                "CategorieJuridique": "5599",
                "IndCategorieJuridique": false,
                "CategorieProfessionnelle": null,
                "IndCategorieProfessionnelle": false,
                "NICSiege": "00020",
                "IndNICSiege": false
            },
            {
                "DateFin": "1991-12-31",
                "DateDebut": "1955-01-01",
                "EtatAdministratif": "A",
                "IndEtatAdministratif": true,
                "Nom": null,
                "Denomination": "CHANVRIERE ABBEVILLOISE",
                "IndDesignation": true,
                "ActivitePrincipale": null,
                "LibelleActivite": null,
                "NomenclatureActivite": null,
                "IndActivitePrincipale": true,
                "CategorieJuridique": "5599",
                "IndCategorieJuridique": true,
                "CategorieProfessionnelle": null,
                "IndCategorieProfessionnelle": true,
                "NICSiege": "00020",
                "IndNICSiege": true
            }
        ]
    }
}
```





<!-- .slide: class="slide" -->
### Exemple de requête sur le siren (2)

GET /ws/siren/005520135?date=2018-01-01

Période courante

```json
{
    "Header": {
        "Statut": 200,
        "Message": "ok"
    },
    "UniteLegale": {
        "Siren": "005520135",
        "StatutDiffusionUniteLegale": "O",
        "DateCreationUniteLegale": "1955-01-01",
        "Sigle": null,
        "Sexe": null,
        "NomUsage": null,
        "Prenom1": null,
        "Prenom2": null,
        "Prenom3": null,
        "Prenom4": null,
        "PrenomUsuel": null,
        "CaractereEmployeur": "O",
        "TrancheEffectifsUniteLegale": "NN",
        "AnneeEffectifsUniteLegale": null,
        "NombrePeriodes": 6,
        "Periodes": [
            {
                "DateFin": null,
                "DateDebut": "2007-11-19",
                "EtatAdministratif": "C",
                "IndEtatAdministratif": true,
                "Nom": null,
                "Denomination": "CHANVI GESTION",
                "IndDesignation": false,
                "ActivitePrincipale": "74.1J",
                "LibelleActivite": "Administration d'entreprises",
                "NomenclatureActivite": "NAFRev1",
                "IndActivitePrincipale": false,
                "CategorieJuridique": "5710",
                "IndCategorieJuridique": false,
                "CategorieProfessionnelle": null,
                "IndCategorieProfessionnelle": false,
                "NICSiege": "00038",
                "IndNICSiege": false
            }
        ]
    }
}
```





<!-- .slide: class="slide" -->
### Exemple de requête sur le siren (3)

GET /ws/siren/005520135?date=2018-01-01

Période trop ancienne
```json
{
    "Header": {
        "Statut": 404,
        "Message": "Aucun élément trouvé pour le Siren 005520135 et date 1950-01-01"
    }
}
```
