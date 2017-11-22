<!-- .slide: class="chapter" -->
## 3
### Recherche multicritère





<!-- .slide: class="slide" -->
### Présentation des services
Rechercher librement sur toutes les unités légales/établissements à partir d'une ou plusieurs variables contenues dans les informations du répertoire
 - les résultats sont paginés (voir l'en-tête Link pour naviguer)
 - l'export en CSV est toujours possible





<!-- .slide: class="slide" -->
### Recherche sur une variable non historisée
**Syntaxe** : nomVariable:valeur

Toutes les variables sont possibles, sauf LibelleActivite et NomenclatureActivite
 ```
/ws/siret?q=CodeCommuneEtablissement:92046
 ```

```json
{
    "Header": {
        "Statut": 200,
        "Message": "ok",
        "Total": 12348,
        "Debut": 0,
        "Nombre": 20
    },
    "Etablissements": [
        {
            "Siren": "219200466",
            "Nic": "00270",
            "StatutDiffusionEtablissement": "O",
            "DateCreationEtablissement": "1979-12-03",
            "NombrePeriodes": 3,
            "UniteLegale": {
                "StatutDiffusionUniteLegale": "O",
                "DateCreationUniteLegale": "1980-01-01",
                "Sigle": null,
                "Sexe": null,
                "NomUsage": null,
                "Prenom1": null,
                "Prenom2": null,
                "Prenom3": null,
                "Prenom4": null,
                "PrenomUsuel": null,
                "CaractereEmployeur": "O",
                "EtatAdministratif": "A",
                "Nom": null,
                "Denomination": "COMMUNE DE MALAKOFF",
                "ActivitePrincipale": "84.11Z",
                "LibelleActivite": "Administration publique générale",
                "NomenclatureActivite": "NAFRev2",
                "CategorieJuridique": "7210",
                "CategorieProfessionnelle": null,
                "NICSiege": "00015"
            },
            "Adresse": {
                "ComplementAdresseEtablissement": null,
                "NumeroVoieEtablissement": null,
                "IndiceRepetitionEtablissement": null,
                "TypeVoieEtablissement": "RUE",
                "LibelleVoieEtablissement": "I ET F JOLIOT CURIE",
                "CodePostalEtablissement": "92240",
                "LibelleCommuneEtablissement": "MALAKOFF",
                "LibelleCommuneEtrangerEtablissement": null,
                "DistributionSpecialeEtablissement": null,
                "CodeCommuneEtablissement": "92046",
                "CedexEtablissement": null
            },
            "Periodes": [
                {
                    "DateFin": null,
                    "DateDebut": "2008-01-01",
                    "EtatAdministratifEtablissement": "A",
                    "IndEtatAdministratifEtablissement": false,
                    "ActivitePrincipaleEtablissement": "87.10A",
                    "LibelleActiviteEtablissement": "Hébergement médicalisé pour personnes âgées",
                    "NomenclatureActiviteEtablissement": "NAFRev2",
                    "IndActivitePrincipaleEtablissement": true,
                    "CaractereEmployeurEtablissement": "N",
                    "IndCaractereEmployeurEtablissement": false,
                    "Enseigne1": "LOGEMENT FOYER JOLIOT CURIE",
                    "Enseigne2": null,
                    "Enseigne3": null,
                    "IndEnseigneEtablissement": false
                },
                {
                    "DateFin": "2007-12-31",
                    "DateDebut": "1979-12-25",
                    "EtatAdministratifEtablissement": "A",
                    "IndEtatAdministratifEtablissement": false,
                    "ActivitePrincipaleEtablissement": "85.3D",
                    "LibelleActiviteEtablissement": "Accueil des personnes âgées",
                    "NomenclatureActiviteEtablissement": "NAF1993",
                    "IndActivitePrincipaleEtablissement": true,
                    "CaractereEmployeurEtablissement": "N",
                    "IndCaractereEmployeurEtablissement": false,
                    "Enseigne1": "LOGEMENT FOYER JOLIOT CURIE",
                    "Enseigne2": null,
                    "Enseigne3": null,
                    "IndEnseigneEtablissement": false
                },
                {
                    "DateFin": "1979-12-24",
                    "DateDebut": "1979-12-03",
                    "EtatAdministratifEtablissement": "A",
                    "IndEtatAdministratifEtablissement": true,
                    "ActivitePrincipaleEtablissement": null,
                    "LibelleActiviteEtablissement": null,
                    "NomenclatureActiviteEtablissement": null,
                    "IndActivitePrincipaleEtablissement": true,
                    "CaractereEmployeurEtablissement": "N",
                    "IndCaractereEmployeurEtablissement": true,
                    "Enseigne1": "LOGEMENT FOYER JOLIOT CURIE",
                    "Enseigne2": null,
                    "Enseigne3": null,
                    "IndEnseigneEtablissement": true
                }
            ]
        },
        {
            "Siren": "219200466",
            "Nic": "00189",
            "StatutDiffusionEtablissement": "O",
            "DateCreationEtablissement": "1945-01-01",
            "NombrePeriodes": 3,
            "UniteLegale": {
                "StatutDiffusionUniteLegale": "O",
                "DateCreationUniteLegale": "1980-01-01",
                "Sigle": null,
                "Sexe": null,
                "NomUsage": null,
                "Prenom1": null,
                "Prenom2": null,
                "Prenom3": null,
                "Prenom4": null,
                "PrenomUsuel": null,
                "CaractereEmployeur": "O",
                "EtatAdministratif": "A",
                "Nom": null,
                "Denomination": "COMMUNE DE MALAKOFF",
                "ActivitePrincipale": "84.11Z",
                "LibelleActivite": "Administration publique générale",
                "NomenclatureActivite": "NAFRev2",
                "CategorieJuridique": "7210",
                "CategorieProfessionnelle": null,
                "NICSiege": "00015"
            },
            "Adresse": {
                "ComplementAdresseEtablissement": null,
                "NumeroVoieEtablissement": "74",
                "IndiceRepetitionEtablissement": null,
                "TypeVoieEtablissement": "AV",
                "LibelleVoieEtablissement": "PIERRE LAROUSSE",
                "CodePostalEtablissement": "92240",
                "LibelleCommuneEtablissement": "MALAKOFF",
                "LibelleCommuneEtrangerEtablissement": null,
                "DistributionSpecialeEtablissement": null,
                "CodeCommuneEtablissement": "92046",
                "CedexEtablissement": null
            },
            "Periodes": [
                {
                    "DateFin": null,
                    "DateDebut": "2008-01-01",
                    "EtatAdministratifEtablissement": "A",
                    "IndEtatAdministratifEtablissement": false,
                    "ActivitePrincipaleEtablissement": "86.21Z",
                    "LibelleActiviteEtablissement": "Activité des médecins généralistes",
                    "NomenclatureActiviteEtablissement": "NAFRev2",
                    "IndActivitePrincipaleEtablissement": true,
                    "CaractereEmployeurEtablissement": "N",
                    "IndCaractereEmployeurEtablissement": false,
                    "Enseigne1": "CENTRE MUNICIPAL DE SANTE",
                    "Enseigne2": null,
                    "Enseigne3": null,
                    "IndEnseigneEtablissement": false
                },
                {
                    "DateFin": "2007-12-31",
                    "DateDebut": "1945-12-25",
                    "EtatAdministratifEtablissement": "A",
                    "IndEtatAdministratifEtablissement": false,
                    "ActivitePrincipaleEtablissement": "85.1C",
                    "LibelleActiviteEtablissement": "Pratique médicale",
                    "NomenclatureActiviteEtablissement": "NAF1993",
                    "IndActivitePrincipaleEtablissement": true,
                    "CaractereEmployeurEtablissement": "N",
                    "IndCaractereEmployeurEtablissement": false,
                    "Enseigne1": "CENTRE MUNICIPAL DE SANTE",
                    "Enseigne2": null,
                    "Enseigne3": null,
                    "IndEnseigneEtablissement": false
                },
                {
                    "DateFin": "1945-12-24",
                    "DateDebut": "1945-01-01",
                    "EtatAdministratifEtablissement": "A",
                    "IndEtatAdministratifEtablissement": true,
                    "ActivitePrincipaleEtablissement": null,
                    "LibelleActiviteEtablissement": null,
                    "NomenclatureActiviteEtablissement": null,
                    "IndActivitePrincipaleEtablissement": true,
                    "CaractereEmployeurEtablissement": "N",
                    "IndCaractereEmployeurEtablissement": true,
                    "Enseigne1": "CENTRE MUNICIPAL DE SANTE",
                    "Enseigne2": null,
                    "Enseigne3": null,
                    "IndEnseigneEtablissement": true
                }
            ]
        },
        {
            "Siren": "219200466",
            "Nic": "00304",
            "StatutDiffusionEtablissement": "O",
            "DateCreationEtablissement": "2000-12-01",
            "NombrePeriodes": 3,
            "UniteLegale": {
                "StatutDiffusionUniteLegale": "O",
                "DateCreationUniteLegale": "1980-01-01",
                "Sigle": null,
                "Sexe": null,
                "NomUsage": null,
                "Prenom1": null,
                "Prenom2": null,
                "Prenom3": null,
                "Prenom4": null,
                "PrenomUsuel": null,
                "CaractereEmployeur": "O",
                "EtatAdministratif": "A",
                "Nom": null,
                "Denomination": "COMMUNE DE MALAKOFF",
                "ActivitePrincipale": "84.11Z",
                "LibelleActivite": "Administration publique générale",
                "NomenclatureActivite": "NAFRev2",
                "CategorieJuridique": "7210",
                "CategorieProfessionnelle": null,
                "NICSiege": "00015"
            },
            "Adresse": {
                "ComplementAdresseEtablissement": "MAIRIE",
                "NumeroVoieEtablissement": null,
                "IndiceRepetitionEtablissement": null,
                "TypeVoieEtablissement": "PL",
                "LibelleVoieEtablissement": "DU ONZE NOVEMBRE",
                "CodePostalEtablissement": "92240",
                "LibelleCommuneEtablissement": "MALAKOFF",
                "LibelleCommuneEtrangerEtablissement": null,
                "DistributionSpecialeEtablissement": null,
                "CodeCommuneEtablissement": "92046",
                "CedexEtablissement": null
            },
            "Periodes": [
                {
                    "DateFin": null,
                    "DateDebut": "2008-01-01",
                    "EtatAdministratifEtablissement": "A",
                    "IndEtatAdministratifEtablissement": false,
                    "ActivitePrincipaleEtablissement": "37.00Z",
                    "LibelleActiviteEtablissement": "Collecte et traitement des eaux usées",
                    "NomenclatureActiviteEtablissement": "NAFRev2",
                    "IndActivitePrincipaleEtablissement": true,
                    "CaractereEmployeurEtablissement": "N",
                    "IndCaractereEmployeurEtablissement": false,
                    "Enseigne1": "SERVICE ASSAINISSEMENT",
                    "Enseigne2": null,
                    "Enseigne3": null,
                    "IndEnseigneEtablissement": false
                },
                {
                    "DateFin": "2007-12-31",
                    "DateDebut": "2000-12-25",
                    "EtatAdministratifEtablissement": "A",
                    "IndEtatAdministratifEtablissement": false,
                    "ActivitePrincipaleEtablissement": "90.0A",
                    "LibelleActiviteEtablissement": "Epuration des eaux usées",
                    "NomenclatureActiviteEtablissement": "NAF1993",
                    "IndActivitePrincipaleEtablissement": true,
                    "CaractereEmployeurEtablissement": "N",
                    "IndCaractereEmployeurEtablissement": false,
                    "Enseigne1": "SERVICE ASSAINISSEMENT",
                    "Enseigne2": null,
                    "Enseigne3": null,
                    "IndEnseigneEtablissement": false
                },
                {
                    "DateFin": "2000-12-24",
                    "DateDebut": "2000-12-01",
                    "EtatAdministratifEtablissement": "A",
                    "IndEtatAdministratifEtablissement": true,
                    "ActivitePrincipaleEtablissement": null,
                    "LibelleActiviteEtablissement": null,
                    "NomenclatureActiviteEtablissement": null,
                    "IndActivitePrincipaleEtablissement": true,
                    "CaractereEmployeurEtablissement": "N",
                    "IndCaractereEmployeurEtablissement": true,
                    "Enseigne1": "SERVICE ASSAINISSEMENT",
                    "Enseigne2": null,
                    "Enseigne3": null,
                    "IndEnseigneEtablissement": true
                }
            ]
        },
        {
            "Siren": "219200466",
            "Nic": "00098",
            "StatutDiffusionEtablissement": "O",
            "DateCreationEtablissement": "1983-12-21",
            "NombrePeriodes": 3,
            "UniteLegale": {
                "StatutDiffusionUniteLegale": "O",
                "DateCreationUniteLegale": "1980-01-01",
                "Sigle": null,
                "Sexe": null,
                "NomUsage": null,
                "Prenom1": null,
                "Prenom2": null,
                "Prenom3": null,
                "Prenom4": null,
                "PrenomUsuel": null,
                "CaractereEmployeur": "O",
                "EtatAdministratif": "A",
                "Nom": null,
                "Denomination": "COMMUNE DE MALAKOFF",
                "ActivitePrincipale": "84.11Z",
                "LibelleActivite": "Administration publique générale",
                "NomenclatureActivite": "NAFRev2",
                "CategorieJuridique": "7210",
                "CategorieProfessionnelle": null,
                "NICSiege": "00015"
            },
            "Adresse": {
                "ComplementAdresseEtablissement": "7 A 17",
                "NumeroVoieEtablissement": "7",
                "IndiceRepetitionEtablissement": null,
                "TypeVoieEtablissement": "AV",
                "LibelleVoieEtablissement": "DU MAL LECLERC",
                "CodePostalEtablissement": "92240",
                "LibelleCommuneEtablissement": "MALAKOFF",
                "LibelleCommuneEtrangerEtablissement": null,
                "DistributionSpecialeEtablissement": null,
                "CodeCommuneEtablissement": "92046",
                "CedexEtablissement": null
            },
            "Periodes": [
                {
                    "DateFin": null,
                    "DateDebut": "2008-01-01",
                    "EtatAdministratifEtablissement": "A",
                    "IndEtatAdministratifEtablissement": false,
                    "ActivitePrincipaleEtablissement": "85.10Z",
                    "LibelleActiviteEtablissement": "Enseignement pré-primaire",
                    "NomenclatureActiviteEtablissement": "NAFRev2",
                    "IndActivitePrincipaleEtablissement": true,
                    "CaractereEmployeurEtablissement": "N",
                    "IndCaractereEmployeurEtablissement": false,
                    "Enseigne1": "ECOLE MATERNELLE PUBLIQUE G COGNIOT",
                    "Enseigne2": null,
                    "Enseigne3": null,
                    "IndEnseigneEtablissement": false
                },
                {
                    "DateFin": "2007-12-31",
                    "DateDebut": "1983-12-25",
                    "EtatAdministratifEtablissement": "A",
                    "IndEtatAdministratifEtablissement": false,
                    "ActivitePrincipaleEtablissement": "80.1Z",
                    "LibelleActiviteEtablissement": "Enseignement primaire",
                    "NomenclatureActiviteEtablissement": "NAF1993",
                    "IndActivitePrincipaleEtablissement": true,
                    "CaractereEmployeurEtablissement": "N",
                    "IndCaractereEmployeurEtablissement": false,
                    "Enseigne1": "ECOLE MATERNELLE PUBLIQUE G COGNIOT",
                    "Enseigne2": null,
                    "Enseigne3": null,
                    "IndEnseigneEtablissement": false
                },
                {
                    "DateFin": "1983-12-24",
                    "DateDebut": "1983-12-21",
                    "EtatAdministratifEtablissement": "A",
                    "IndEtatAdministratifEtablissement": true,
                    "ActivitePrincipaleEtablissement": null,
                    "LibelleActiviteEtablissement": null,
                    "NomenclatureActiviteEtablissement": null,
                    "IndActivitePrincipaleEtablissement": true,
                    "CaractereEmployeurEtablissement": "N",
                    "IndCaractereEmployeurEtablissement": true,
                    "Enseigne1": "ECOLE MATERNELLE PUBLIQUE G COGNIOT",
                    "Enseigne2": null,
                    "Enseigne3": null,
                    "IndEnseigneEtablissement": true
                }
            ]
        },
        {
            "Siren": "219200466",
            "Nic": "00171",
            "StatutDiffusionEtablissement": "O",
            "DateCreationEtablissement": "1986-11-12",
            "NombrePeriodes": 3,
            "UniteLegale": {
                "StatutDiffusionUniteLegale": "O",
                "DateCreationUniteLegale": "1980-01-01",
                "Sigle": null,
                "Sexe": null,
                "NomUsage": null,
                "Prenom1": null,
                "Prenom2": null,
                "Prenom3": null,
                "Prenom4": null,
                "PrenomUsuel": null,
                "CaractereEmployeur": "O",
                "EtatAdministratif": "A",
                "Nom": null,
                "Denomination": "COMMUNE DE MALAKOFF",
                "ActivitePrincipale": "84.11Z",
                "LibelleActivite": "Administration publique générale",
                "NomenclatureActivite": "NAFRev2",
                "CategorieJuridique": "7210",
                "CategorieProfessionnelle": null,
                "NICSiege": "00015"
            },
            "Adresse": {
                "ComplementAdresseEtablissement": null,
                "NumeroVoieEtablissement": "13",
                "IndiceRepetitionEtablissement": null,
                "TypeVoieEtablissement": "AV",
                "LibelleVoieEtablissement": "JULES FERRY",
                "CodePostalEtablissement": "92240",
                "LibelleCommuneEtablissement": "MALAKOFF",
                "LibelleCommuneEtrangerEtablissement": null,
                "DistributionSpecialeEtablissement": null,
                "CodeCommuneEtablissement": "92046",
                "CedexEtablissement": null
            },
            "Periodes": [
                {
                    "DateFin": null,
                    "DateDebut": "2008-01-01",
                    "EtatAdministratifEtablissement": "A",
                    "IndEtatAdministratifEtablissement": false,
                    "ActivitePrincipaleEtablissement": "85.20Z",
                    "LibelleActiviteEtablissement": "Enseignement primaire",
                    "NomenclatureActiviteEtablissement": "NAFRev2",
                    "IndActivitePrincipaleEtablissement": true,
                    "CaractereEmployeurEtablissement": "N",
                    "IndCaractereEmployeurEtablissement": false,
                    "Enseigne1": "ECOLE PRIMAIRE PUBLIQUE JEAN JAURES",
                    "Enseigne2": null,
                    "Enseigne3": null,
                    "IndEnseigneEtablissement": false
                },
                {
                    "DateFin": "2007-12-31",
                    "DateDebut": "1986-12-25",
                    "EtatAdministratifEtablissement": "A",
                    "IndEtatAdministratifEtablissement": false,
                    "ActivitePrincipaleEtablissement": "80.1Z",
                    "LibelleActiviteEtablissement": "Enseignement primaire",
                    "NomenclatureActiviteEtablissement": "NAF1993",
                    "IndActivitePrincipaleEtablissement": true,
                    "CaractereEmployeurEtablissement": "N",
                    "IndCaractereEmployeurEtablissement": false,
                    "Enseigne1": "ECOLE PRIMAIRE PUBLIQUE JEAN JAURES",
                    "Enseigne2": null,
                    "Enseigne3": null,
                    "IndEnseigneEtablissement": false
                },
                {
                    "DateFin": "1986-12-24",
                    "DateDebut": "1986-11-12",
                    "EtatAdministratifEtablissement": "A",
                    "IndEtatAdministratifEtablissement": true,
                    "ActivitePrincipaleEtablissement": null,
                    "LibelleActiviteEtablissement": null,
                    "NomenclatureActiviteEtablissement": null,
                    "IndActivitePrincipaleEtablissement": true,
                    "CaractereEmployeurEtablissement": "N",
                    "IndCaractereEmployeurEtablissement": true,
                    "Enseigne1": "ECOLE PRIMAIRE PUBLIQUE JEAN JAURES",
                    "Enseigne2": null,
                    "Enseigne3": null,
                    "IndEnseigneEtablissement": true
                }
            ]
        },
        {
            "Siren": "219200466",
            "Nic": "00254",
            "StatutDiffusionEtablissement": "O",
            "DateCreationEtablissement": "1981-09-15",
            "NombrePeriodes": 3,
            "UniteLegale": {
                "StatutDiffusionUniteLegale": "O",
                "DateCreationUniteLegale": "1980-01-01",
                "Sigle": null,
                "Sexe": null,
                "NomUsage": null,
                "Prenom1": null,
                "Prenom2": null,
                "Prenom3": null,
                "Prenom4": null,
                "PrenomUsuel": null,
                "CaractereEmployeur": "O",
                "EtatAdministratif": "A",
                "Nom": null,
                "Denomination": "COMMUNE DE MALAKOFF",
                "ActivitePrincipale": "84.11Z",
                "LibelleActivite": "Administration publique générale",
                "NomenclatureActivite": "NAFRev2",
                "CategorieJuridique": "7210",
                "CategorieProfessionnelle": null,
                "NICSiege": "00015"
            },
            "Adresse": {
                "ComplementAdresseEtablissement": null,
                "NumeroVoieEtablissement": "23",
                "IndiceRepetitionEtablissement": null,
                "TypeVoieEtablissement": "RUE",
                "LibelleVoieEtablissement": "VOLTAIRE",
                "CodePostalEtablissement": "92240",
                "LibelleCommuneEtablissement": "MALAKOFF",
                "LibelleCommuneEtrangerEtablissement": null,
                "DistributionSpecialeEtablissement": null,
                "CodeCommuneEtablissement": "92046",
                "CedexEtablissement": null
            },
            "Periodes": [
                {
                    "DateFin": null,
                    "DateDebut": "2008-01-01",
                    "EtatAdministratifEtablissement": "A",
                    "IndEtatAdministratifEtablissement": false,
                    "ActivitePrincipaleEtablissement": "88.91A",
                    "LibelleActiviteEtablissement": "Accueil de jeunes enfants",
                    "NomenclatureActiviteEtablissement": "NAFRev2",
                    "IndActivitePrincipaleEtablissement": true,
                    "CaractereEmployeurEtablissement": "N",
                    "IndCaractereEmployeurEtablissement": false,
                    "Enseigne1": "CRECHE FAMILIALE MUNICIPALE",
                    "Enseigne2": null,
                    "Enseigne3": null,
                    "IndEnseigneEtablissement": false
                },
                {
                    "DateFin": "2007-12-31",
                    "DateDebut": "1981-12-25",
                    "EtatAdministratifEtablissement": "A",
                    "IndEtatAdministratifEtablissement": false,
                    "ActivitePrincipaleEtablissement": "85.3G",
                    "LibelleActiviteEtablissement": "Crèches et garderies d'enfants",
                    "NomenclatureActiviteEtablissement": "NAF1993",
                    "IndActivitePrincipaleEtablissement": true,
                    "CaractereEmployeurEtablissement": "N",
                    "IndCaractereEmployeurEtablissement": false,
                    "Enseigne1": "CRECHE FAMILIALE MUNICIPALE",
                    "Enseigne2": null,
                    "Enseigne3": null,
                    "IndEnseigneEtablissement": false
                },
                {
                    "DateFin": "1981-12-24",
                    "DateDebut": "1981-09-15",
                    "EtatAdministratifEtablissement": "A",
                    "IndEtatAdministratifEtablissement": true,
                    "ActivitePrincipaleEtablissement": null,
                    "LibelleActiviteEtablissement": null,
                    "NomenclatureActiviteEtablissement": null,
                    "IndActivitePrincipaleEtablissement": true,
                    "CaractereEmployeurEtablissement": "N",
                    "IndCaractereEmployeurEtablissement": true,
                    "Enseigne1": "CRECHE FAMILIALE MUNICIPALE",
                    "Enseigne2": null,
                    "Enseigne3": null,
                    "IndEnseigneEtablissement": true
                }
            ]
        },
        {
            "Siren": "300573193",
            "Nic": "00061",
            "StatutDiffusionEtablissement": "O",
            "DateCreationEtablissement": "1999-03-01",
            "NombrePeriodes": 6,
            "UniteLegale": {
                "StatutDiffusionUniteLegale": "O",
                "DateCreationUniteLegale": "1900-01-01",
                "Sigle": null,
                "Sexe": null,
                "NomUsage": null,
                "Prenom1": null,
                "Prenom2": null,
                "Prenom3": null,
                "Prenom4": null,
                "PrenomUsuel": null,
                "CaractereEmployeur": "O",
                "EtatAdministratif": "A",
                "Nom": null,
                "Denomination": "CCF",
                "ActivitePrincipale": "46.51Z",
                "LibelleActivite": "Commerce de gros (commerce interentreprises) d'ordinateurs, d'équipements informatiques périphériques et de logiciels",
                "NomenclatureActivite": "NAFRev2",
                "CategorieJuridique": "5720",
                "CategorieProfessionnelle": null,
                "NICSiege": "00160"
            },
            "Adresse": {
                "ComplementAdresseEtablissement": null,
                "NumeroVoieEtablissement": "114",
                "IndiceRepetitionEtablissement": null,
                "TypeVoieEtablissement": "AV",
                "LibelleVoieEtablissement": "PIERRE BROSSOLETTE",
                "CodePostalEtablissement": "92240",
                "LibelleCommuneEtablissement": "MALAKOFF",
                "LibelleCommuneEtrangerEtablissement": null,
                "DistributionSpecialeEtablissement": null,
                "CodeCommuneEtablissement": "92046",
                "CedexEtablissement": null
            },
            "Periodes": [
                {
                    "DateFin": null,
                    "DateDebut": "2007-05-23",
                    "EtatAdministratifEtablissement": "F",
                    "IndEtatAdministratifEtablissement": true,
                    "ActivitePrincipaleEtablissement": "51.8L",
                    "LibelleActiviteEtablissement": "Commerce de gros de matériel électrique",
                    "NomenclatureActiviteEtablissement": "NAFRev1",
                    "IndActivitePrincipaleEtablissement": false,
                    "CaractereEmployeurEtablissement": "O",
                    "IndCaractereEmployeurEtablissement": false,
                    "Enseigne1": null,
                    "Enseigne2": null,
                    "Enseigne3": null,
                    "IndEnseigneEtablissement": false
                },
                {
                    "DateFin": "2007-05-22",
                    "DateDebut": "2006-09-13",
                    "EtatAdministratifEtablissement": "A",
                    "IndEtatAdministratifEtablissement": false,
                    "ActivitePrincipaleEtablissement": "51.8L",
                    "LibelleActiviteEtablissement": "Commerce de gros de matériel électrique",
                    "NomenclatureActiviteEtablissement": "NAFRev1",
                    "IndActivitePrincipaleEtablissement": true,
                    "CaractereEmployeurEtablissement": "O",
                    "IndCaractereEmployeurEtablissement": false,
                    "Enseigne1": null,
                    "Enseigne2": null,
                    "Enseigne3": null,
                    "IndEnseigneEtablissement": false
                },
                {
                    "DateFin": "2006-09-12",
                    "DateDebut": "2005-01-01",
                    "EtatAdministratifEtablissement": "A",
                    "IndEtatAdministratifEtablissement": false,
                    "ActivitePrincipaleEtablissement": "51.8J",
                    "LibelleActiviteEtablissement": "Commerce de gros de composants et d'autres équipements électroniques",
                    "NomenclatureActiviteEtablissement": "NAFRev1",
                    "IndActivitePrincipaleEtablissement": false,
                    "CaractereEmployeurEtablissement": "O",
                    "IndCaractereEmployeurEtablissement": true,
                    "Enseigne1": null,
                    "Enseigne2": null,
                    "Enseigne3": null,
                    "IndEnseigneEtablissement": false
                },
                {
                    "DateFin": "2004-12-31",
                    "DateDebut": "2003-12-25",
                    "EtatAdministratifEtablissement": "A",
                    "IndEtatAdministratifEtablissement": false,
                    "ActivitePrincipaleEtablissement": "51.8J",
                    "LibelleActiviteEtablissement": "Commerce de gros de composants et d'autres équipements électroniques",
                    "NomenclatureActiviteEtablissement": "NAFRev1",
                    "IndActivitePrincipaleEtablissement": true,
                    "CaractereEmployeurEtablissement": "N",
                    "IndCaractereEmployeurEtablissement": false,
                    "Enseigne1": null,
                    "Enseigne2": null,
                    "Enseigne3": null,
                    "IndEnseigneEtablissement": false
                },
                {
                    "DateFin": "2003-12-24",
                    "DateDebut": "1999-12-25",
                    "EtatAdministratifEtablissement": "A",
                    "IndEtatAdministratifEtablissement": false,
                    "ActivitePrincipaleEtablissement": "51.6J",
                    "LibelleActiviteEtablissement": "Commerce de gros de matériel électrique et électronique",
                    "NomenclatureActiviteEtablissement": "NAF1993",
                    "IndActivitePrincipaleEtablissement": true,
                    "CaractereEmployeurEtablissement": "N",
                    "IndCaractereEmployeurEtablissement": false,
                    "Enseigne1": null,
                    "Enseigne2": null,
                    "Enseigne3": null,
                    "IndEnseigneEtablissement": false
                },
                {
                    "DateFin": "1999-12-24",
                    "DateDebut": "1999-03-01",
                    "EtatAdministratifEtablissement": "A",
                    "IndEtatAdministratifEtablissement": true,
                    "ActivitePrincipaleEtablissement": null,
                    "LibelleActiviteEtablissement": null,
                    "NomenclatureActiviteEtablissement": null,
                    "IndActivitePrincipaleEtablissement": true,
                    "CaractereEmployeurEtablissement": "N",
                    "IndCaractereEmployeurEtablissement": true,
                    "Enseigne1": null,
                    "Enseigne2": null,
                    "Enseigne3": null,
                    "IndEnseigneEtablissement": true
                }
            ]
        },
        {
            "Siren": "279200364",
            "Nic": "00024",
            "StatutDiffusionEtablissement": "O",
            "DateCreationEtablissement": "1985-12-23",
            "NombrePeriodes": 4,
            "UniteLegale": {
                "StatutDiffusionUniteLegale": "O",
                "DateCreationUniteLegale": "1927-01-01",
                "Sigle": "OPH MALAKOFF",
                "Sexe": null,
                "NomUsage": null,
                "Prenom1": null,
                "Prenom2": null,
                "Prenom3": null,
                "Prenom4": null,
                "PrenomUsuel": null,
                "CaractereEmployeur": "O",
                "EtatAdministratif": "A",
                "Nom": null,
                "Denomination": "OFFICE PUBLIC DE L'HABITAT DE MALAKOFF",
                "ActivitePrincipale": "68.20A",
                "LibelleActivite": "Location de logements",
                "NomenclatureActivite": "NAFRev2",
                "CategorieJuridique": "4140",
                "CategorieProfessionnelle": null,
                "NICSiege": "00024"
            },
            "Adresse": {
                "ComplementAdresseEtablissement": null,
                "NumeroVoieEtablissement": "2",
                "IndiceRepetitionEtablissement": null,
                "TypeVoieEtablissement": "RUE",
                "LibelleVoieEtablissement": "JEAN LURCAT",
                "CodePostalEtablissement": "92240",
                "LibelleCommuneEtablissement": "MALAKOFF",
                "LibelleCommuneEtrangerEtablissement": null,
                "DistributionSpecialeEtablissement": null,
                "CodeCommuneEtablissement": "92046",
                "CedexEtablissement": null
            },
            "Periodes": [
                {
                    "DateFin": null,
                    "DateDebut": "2008-01-01",
                    "EtatAdministratifEtablissement": "A",
                    "IndEtatAdministratifEtablissement": false,
                    "ActivitePrincipaleEtablissement": "68.20A",
                    "LibelleActiviteEtablissement": "Location de logements",
                    "NomenclatureActiviteEtablissement": "NAFRev2",
                    "IndActivitePrincipaleEtablissement": true,
                    "CaractereEmployeurEtablissement": "O",
                    "IndCaractereEmployeurEtablissement": false,
                    "Enseigne1": null,
                    "Enseigne2": null,
                    "Enseigne3": null,
                    "IndEnseigneEtablissement": false
                },
                {
                    "DateFin": "2007-12-31",
                    "DateDebut": "2003-12-25",
                    "EtatAdministratifEtablissement": "A",
                    "IndEtatAdministratifEtablissement": false,
                    "ActivitePrincipaleEtablissement": "70.2A",
                    "LibelleActiviteEtablissement": "Location de logements",
                    "NomenclatureActiviteEtablissement": "NAFRev1",
                    "IndActivitePrincipaleEtablissement": true,
                    "CaractereEmployeurEtablissement": "O",
                    "IndCaractereEmployeurEtablissement": false,
                    "Enseigne1": null,
                    "Enseigne2": null,
                    "Enseigne3": null,
                    "IndEnseigneEtablissement": false
                },
                {
                    "DateFin": "2003-12-24",
                    "DateDebut": "1996-12-25",
                    "EtatAdministratifEtablissement": "A",
                    "IndEtatAdministratifEtablissement": false,
                    "ActivitePrincipaleEtablissement": null,
                    "LibelleActiviteEtablissement": null,
                    "NomenclatureActiviteEtablissement": null,
                    "IndActivitePrincipaleEtablissement": false,
                    "CaractereEmployeurEtablissement": "O",
                    "IndCaractereEmployeurEtablissement": true,
                    "Enseigne1": null,
                    "Enseigne2": null,
                    "Enseigne3": null,
                    "IndEnseigneEtablissement": false
                },
                {
                    "DateFin": "1996-12-24",
                    "DateDebut": "1985-12-23",
                    "EtatAdministratifEtablissement": "A",
                    "IndEtatAdministratifEtablissement": true,
                    "ActivitePrincipaleEtablissement": null,
                    "LibelleActiviteEtablissement": null,
                    "NomenclatureActiviteEtablissement": null,
                    "IndActivitePrincipaleEtablissement": true,
                    "CaractereEmployeurEtablissement": null,
                    "IndCaractereEmployeurEtablissement": true,
                    "Enseigne1": null,
                    "Enseigne2": null,
                    "Enseigne3": null,
                    "IndEnseigneEtablissement": true
                }
            ]
        },
        {
            "Siren": "300581493",
            "Nic": "00016",
            "StatutDiffusionEtablissement": "O",
            "DateCreationEtablissement": null,
            "NombrePeriodes": 1,
            "UniteLegale": {
                "StatutDiffusionUniteLegale": "O",
                "DateCreationUniteLegale": "1972-12-25",
                "Sigle": null,
                "Sexe": 2,
                "NomUsage": "LEGOUI",
                "Prenom1": "RAYMONDE",
                "Prenom2": null,
                "Prenom3": null,
                "Prenom4": null,
                "PrenomUsuel": "RAYMONDE",
                "CaractereEmployeur": "N",
                "UnitePurgee": true,
                "EtatAdministratif": "C",
                "Nom": "MOUFFLET",
                "Denomination": null,
                "ActivitePrincipale": "93.0D",
                "LibelleActivite": "Coiffure",
                "NomenclatureActivite": "NAFRev1",
                "CategorieJuridique": null,
                "CategorieProfessionnelle": "1000",
                "NICSiege": "00016"
            },
            "Adresse": {
                "ComplementAdresseEtablissement": null,
                "NumeroVoieEtablissement": "41",
                "IndiceRepetitionEtablissement": null,
                "TypeVoieEtablissement": "RUE",
                "LibelleVoieEtablissement": "PAUL BERT",
                "CodePostalEtablissement": "92240",
                "LibelleCommuneEtablissement": "MALAKOFF",
                "LibelleCommuneEtrangerEtablissement": null,
                "DistributionSpecialeEtablissement": null,
                "CodeCommuneEtablissement": "92046",
                "CedexEtablissement": null
            },
            "Periodes": [
                {
                    "DateFin": null,
                    "DateDebut": "1992-05-30",
                    "EtatAdministratifEtablissement": "F",
                    "IndEtatAdministratifEtablissement": true,
                    "ActivitePrincipaleEtablissement": "93.0D",
                    "LibelleActiviteEtablissement": "Coiffure",
                    "NomenclatureActiviteEtablissement": "NAF1993",
                    "IndActivitePrincipaleEtablissement": false,
                    "CaractereEmployeurEtablissement": "N",
                    "IndCaractereEmployeurEtablissement": false,
                    "Enseigne1": null,
                    "Enseigne2": null,
                    "Enseigne3": null,
                    "IndEnseigneEtablissement": false
                }
            ]
        },
        {
            "Siren": "303952402",
            "Nic": "00012",
            "StatutDiffusionEtablissement": "O",
            "DateCreationEtablissement": "1900-01-01",
            "NombrePeriodes": 5,
            "UniteLegale": {
                "StatutDiffusionUniteLegale": "O",
                "DateCreationUniteLegale": "1900-01-01",
                "Sigle": null,
                "Sexe": null,
                "NomUsage": null,
                "Prenom1": null,
                "Prenom2": null,
                "Prenom3": null,
                "Prenom4": null,
                "PrenomUsuel": null,
                "CaractereEmployeur": "O",
                "EtatAdministratif": "A",
                "Nom": null,
                "Denomination": "ENTREPRISE KASPARIAN",
                "ActivitePrincipale": "43.99A",
                "LibelleActivite": "Travaux d'étanchéification",
                "NomenclatureActivite": "NAFRev2",
                "CategorieJuridique": "5499",
                "CategorieProfessionnelle": null,
                "NICSiege": "00020"
            },
            "Adresse": {
                "ComplementAdresseEtablissement": null,
                "NumeroVoieEtablissement": "10",
                "IndiceRepetitionEtablissement": null,
                "TypeVoieEtablissement": "RUE",
                "LibelleVoieEtablissement": "LOUIS GIRARD",
                "CodePostalEtablissement": "92240",
                "LibelleCommuneEtablissement": "MALAKOFF",
                "LibelleCommuneEtrangerEtablissement": null,
                "DistributionSpecialeEtablissement": null,
                "CodeCommuneEtablissement": "92046",
                "CedexEtablissement": null
            },
            "Periodes": [
                {
                    "DateFin": null,
                    "DateDebut": "2014-09-01",
                    "EtatAdministratifEtablissement": "F",
                    "IndEtatAdministratifEtablissement": true,
                    "ActivitePrincipaleEtablissement": "43.99A",
                    "LibelleActiviteEtablissement": "Travaux d'étanchéification",
                    "NomenclatureActiviteEtablissement": "NAFRev2",
                    "IndActivitePrincipaleEtablissement": false,
                    "CaractereEmployeurEtablissement": "O",
                    "IndCaractereEmployeurEtablissement": false,
                    "Enseigne1": null,
                    "Enseigne2": null,
                    "Enseigne3": null,
                    "IndEnseigneEtablissement": false
                },
                {
                    "DateFin": "2014-08-31",
                    "DateDebut": "2008-01-01",
                    "EtatAdministratifEtablissement": "A",
                    "IndEtatAdministratifEtablissement": false,
                    "ActivitePrincipaleEtablissement": "43.99A",
                    "LibelleActiviteEtablissement": "Travaux d'étanchéification",
                    "NomenclatureActiviteEtablissement": "NAFRev2",
                    "IndActivitePrincipaleEtablissement": true,
                    "CaractereEmployeurEtablissement": "O",
                    "IndCaractereEmployeurEtablissement": false,
                    "Enseigne1": null,
                    "Enseigne2": null,
                    "Enseigne3": null,
                    "IndEnseigneEtablissement": false
                },
                {
                    "DateFin": "2007-12-31",
                    "DateDebut": "1996-12-25",
                    "EtatAdministratifEtablissement": "A",
                    "IndEtatAdministratifEtablissement": false,
                    "ActivitePrincipaleEtablissement": "45.2K",
                    "LibelleActiviteEtablissement": "Travaux d'étanchéification",
                    "NomenclatureActiviteEtablissement": "NAF1993",
                    "IndActivitePrincipaleEtablissement": false,
                    "CaractereEmployeurEtablissement": "O",
                    "IndCaractereEmployeurEtablissement": true,
                    "Enseigne1": null,
                    "Enseigne2": null,
                    "Enseigne3": null,
                    "IndEnseigneEtablissement": false
                },
                {
                    "DateFin": "1996-12-24",
                    "DateDebut": "1991-12-25",
                    "EtatAdministratifEtablissement": "A",
                    "IndEtatAdministratifEtablissement": false,
                    "ActivitePrincipaleEtablissement": "45.2K",
                    "LibelleActiviteEtablissement": "Travaux d'étanchéification",
                    "NomenclatureActiviteEtablissement": "NAF1993",
                    "IndActivitePrincipaleEtablissement": true,
                    "CaractereEmployeurEtablissement": null,
                    "IndCaractereEmployeurEtablissement": false,
                    "Enseigne1": null,
                    "Enseigne2": null,
                    "Enseigne3": null,
                    "IndEnseigneEtablissement": false
                },
                {
                    "DateFin": "1991-12-24",
                    "DateDebut": "1900-01-01",
                    "EtatAdministratifEtablissement": "A",
                    "IndEtatAdministratifEtablissement": true,
                    "ActivitePrincipaleEtablissement": null,
                    "LibelleActiviteEtablissement": null,
                    "NomenclatureActiviteEtablissement": null,
                    "IndActivitePrincipaleEtablissement": true,
                    "CaractereEmployeurEtablissement": null,
                    "IndCaractereEmployeurEtablissement": true,
                    "Enseigne1": null,
                    "Enseigne2": null,
                    "Enseigne3": null,
                    "IndEnseigneEtablissement": true
                }
            ]
        },
        {
            "Siren": "304176522",
            "Nic": "00015",
            "StatutDiffusionEtablissement": "O",
            "DateCreationEtablissement": "1900-01-01",
            "NombrePeriodes": 3,
            "UniteLegale": {
                "StatutDiffusionUniteLegale": "O",
                "DateCreationUniteLegale": "1900-01-01",
                "Sigle": null,
                "Sexe": 2,
                "NomUsage": null,
                "Prenom1": "ROSA",
                "Prenom2": null,
                "Prenom3": null,
                "Prenom4": null,
                "PrenomUsuel": "ROSA",
                "CaractereEmployeur": "N",
                "EtatAdministratif": "A",
                "Nom": "OSMAN",
                "Denomination": null,
                "ActivitePrincipale": "47.89Z",
                "LibelleActivite": "Autres commerces de détail sur éventaires et marchés",
                "NomenclatureActivite": "NAFRev2",
                "CategorieJuridique": null,
                "CategorieProfessionnelle": "1000",
                "NICSiege": "00015"
            },
            "Adresse": {
                "ComplementAdresseEtablissement": null,
                "NumeroVoieEtablissement": "29",
                "IndiceRepetitionEtablissement": null,
                "TypeVoieEtablissement": "RUE",
                "LibelleVoieEtablissement": "GALLIENI",
                "CodePostalEtablissement": "92240",
                "LibelleCommuneEtablissement": "MALAKOFF",
                "LibelleCommuneEtrangerEtablissement": null,
                "DistributionSpecialeEtablissement": null,
                "CodeCommuneEtablissement": "92046",
                "CedexEtablissement": null
            },
            "Periodes": [
                {
                    "DateFin": null,
                    "DateDebut": "2008-01-01",
                    "EtatAdministratifEtablissement": "A",
                    "IndEtatAdministratifEtablissement": false,
                    "ActivitePrincipaleEtablissement": "47.89Z",
                    "LibelleActiviteEtablissement": "Autres commerces de détail sur éventaires et marchés",
                    "NomenclatureActiviteEtablissement": "NAFRev2",
                    "IndActivitePrincipaleEtablissement": true,
                    "CaractereEmployeurEtablissement": "N",
                    "IndCaractereEmployeurEtablissement": false,
                    "Enseigne1": null,
                    "Enseigne2": null,
                    "Enseigne3": null,
                    "IndEnseigneEtablissement": false
                },
                {
                    "DateFin": "2007-12-31",
                    "DateDebut": "1988-12-25",
                    "EtatAdministratifEtablissement": "A",
                    "IndEtatAdministratifEtablissement": false,
                    "ActivitePrincipaleEtablissement": "52.6E",
                    "LibelleActiviteEtablissement": "Commerce de détail non alimentaire sur éventaires et marchés",
                    "NomenclatureActiviteEtablissement": "NAF1993",
                    "IndActivitePrincipaleEtablissement": true,
                    "CaractereEmployeurEtablissement": "N",
                    "IndCaractereEmployeurEtablissement": false,
                    "Enseigne1": null,
                    "Enseigne2": null,
                    "Enseigne3": null,
                    "IndEnseigneEtablissement": false
                },
                {
                    "DateFin": "1988-12-24",
                    "DateDebut": "1900-01-01",
                    "EtatAdministratifEtablissement": "A",
                    "IndEtatAdministratifEtablissement": true,
                    "ActivitePrincipaleEtablissement": null,
                    "LibelleActiviteEtablissement": null,
                    "NomenclatureActiviteEtablissement": null,
                    "IndActivitePrincipaleEtablissement": true,
                    "CaractereEmployeurEtablissement": "N",
                    "IndCaractereEmployeurEtablissement": true,
                    "Enseigne1": null,
                    "Enseigne2": null,
                    "Enseigne3": null,
                    "IndEnseigneEtablissement": true
                }
            ]
        },
        {
            "Siren": "303015093",
            "Nic": "00030",
            "StatutDiffusionEtablissement": "O",
            "DateCreationEtablissement": "2002-10-01",
            "NombrePeriodes": 5,
            "UniteLegale": {
                "StatutDiffusionUniteLegale": "O",
                "DateCreationUniteLegale": "1959-01-01",
                "Sigle": null,
                "Sexe": null,
                "NomUsage": null,
                "Prenom1": null,
                "Prenom2": null,
                "Prenom3": null,
                "Prenom4": null,
                "PrenomUsuel": null,
                "CaractereEmployeur": "N",
                "EtatAdministratif": "C",
                "Nom": null,
                "Denomination": "SOC LE LOGIS IDEAL",
                "ActivitePrincipale": "68.20A",
                "LibelleActivite": "Location de logements",
                "NomenclatureActivite": "NAFRev2",
                "CategorieJuridique": "5499",
                "CategorieProfessionnelle": null,
                "NICSiege": "00030"
            },
            "Adresse": {
                "ComplementAdresseEtablissement": null,
                "NumeroVoieEtablissement": "14",
                "IndiceRepetitionEtablissement": null,
                "TypeVoieEtablissement": "RUE",
                "LibelleVoieEtablissement": "AVAULEE",
                "CodePostalEtablissement": "92240",
                "LibelleCommuneEtablissement": "MALAKOFF",
                "LibelleCommuneEtrangerEtablissement": null,
                "DistributionSpecialeEtablissement": null,
                "CodeCommuneEtablissement": "92046",
                "CedexEtablissement": null
            },
            "Periodes": [
                {
                    "DateFin": null,
                    "DateDebut": "2015-11-29",
                    "EtatAdministratifEtablissement": "F",
                    "IndEtatAdministratifEtablissement": true,
                    "ActivitePrincipaleEtablissement": "68.20A",
                    "LibelleActiviteEtablissement": "Location de logements",
                    "NomenclatureActiviteEtablissement": "NAFRev2",
                    "IndActivitePrincipaleEtablissement": false,
                    "CaractereEmployeurEtablissement": "N",
                    "IndCaractereEmployeurEtablissement": false,
                    "Enseigne1": null,
                    "Enseigne2": null,
                    "Enseigne3": null,
                    "IndEnseigneEtablissement": false
                },
                {
                    "DateFin": "2015-11-28",
                    "DateDebut": "2008-01-01",
                    "EtatAdministratifEtablissement": "A",
                    "IndEtatAdministratifEtablissement": false,
                    "ActivitePrincipaleEtablissement": "68.20A",
                    "LibelleActiviteEtablissement": "Location de logements",
                    "NomenclatureActiviteEtablissement": "NAFRev2",
                    "IndActivitePrincipaleEtablissement": true,
                    "CaractereEmployeurEtablissement": "N",
                    "IndCaractereEmployeurEtablissement": false,
                    "Enseigne1": null,
                    "Enseigne2": null,
                    "Enseigne3": null,
                    "IndEnseigneEtablissement": false
                },
                {
                    "DateFin": "2007-12-31",
                    "DateDebut": "2007-12-31",
                    "EtatAdministratifEtablissement": "A",
                    "IndEtatAdministratifEtablissement": false,
                    "ActivitePrincipaleEtablissement": "70.2A",
                    "LibelleActiviteEtablissement": "Location de logements",
                    "NomenclatureActiviteEtablissement": "NAFRev1",
                    "IndActivitePrincipaleEtablissement": false,
                    "CaractereEmployeurEtablissement": "N",
                    "IndCaractereEmployeurEtablissement": true,
                    "Enseigne1": null,
                    "Enseigne2": null,
                    "Enseigne3": null,
                    "IndEnseigneEtablissement": false
                },
                {
                    "DateFin": "2007-12-30",
                    "DateDebut": "2002-12-25",
                    "EtatAdministratifEtablissement": "A",
                    "IndEtatAdministratifEtablissement": false,
                    "ActivitePrincipaleEtablissement": "70.2A",
                    "LibelleActiviteEtablissement": "Location de logements",
                    "NomenclatureActiviteEtablissement": "NAF1993",
                    "IndActivitePrincipaleEtablissement": true,
                    "CaractereEmployeurEtablissement": "O",
                    "IndCaractereEmployeurEtablissement": true,
                    "Enseigne1": null,
                    "Enseigne2": null,
                    "Enseigne3": null,
                    "IndEnseigneEtablissement": false
                },
                {
                    "DateFin": "2002-12-24",
                    "DateDebut": "2002-10-01",
                    "EtatAdministratifEtablissement": "A",
                    "IndEtatAdministratifEtablissement": true,
                    "ActivitePrincipaleEtablissement": null,
                    "LibelleActiviteEtablissement": null,
                    "NomenclatureActiviteEtablissement": null,
                    "IndActivitePrincipaleEtablissement": true,
                    "CaractereEmployeurEtablissement": null,
                    "IndCaractereEmployeurEtablissement": true,
                    "Enseigne1": null,
                    "Enseigne2": null,
                    "Enseigne3": null,
                    "IndEnseigneEtablissement": true
                }
            ]
        },
        {
            "Siren": "303069744",
            "Nic": "00017",
            "StatutDiffusionEtablissement": "O",
            "DateCreationEtablissement": null,
            "NombrePeriodes": 1,
            "UniteLegale": {
                "StatutDiffusionUniteLegale": "O",
                "DateCreationUniteLegale": "1900-01-01",
                "Sigle": null,
                "Sexe": null,
                "NomUsage": null,
                "Prenom1": null,
                "Prenom2": null,
                "Prenom3": null,
                "Prenom4": null,
                "PrenomUsuel": null,
                "CaractereEmployeur": "N",
                "UnitePurgee": true,
                "EtatAdministratif": "C",
                "Nom": null,
                "Denomination": "CALMELS S DE FAIT",
                "ActivitePrincipale": "67.07",
                "LibelleActivite": "Cafés associés à une autre activité",
                "NomenclatureActivite": "NAP",
                "CategorieJuridique": "9900",
                "CategorieProfessionnelle": null,
                "NICSiege": "00017"
            },
            "Adresse": {
                "ComplementAdresseEtablissement": null,
                "NumeroVoieEtablissement": "51",
                "IndiceRepetitionEtablissement": null,
                "TypeVoieEtablissement": "AV",
                "LibelleVoieEtablissement": "AUGUSTIN DUMONT",
                "CodePostalEtablissement": "92240",
                "LibelleCommuneEtablissement": "MALAKOFF",
                "LibelleCommuneEtrangerEtablissement": null,
                "DistributionSpecialeEtablissement": null,
                "CodeCommuneEtablissement": "92046",
                "CedexEtablissement": null
            },
            "Periodes": [
                {
                    "DateFin": null,
                    "DateDebut": null,
                    "EtatAdministratifEtablissement": "F",
                    "IndEtatAdministratifEtablissement": false,
                    "ActivitePrincipaleEtablissement": "67.07",
                    "LibelleActiviteEtablissement": "Cafés associés à une autre activité",
                    "NomenclatureActiviteEtablissement": "NAP",
                    "IndActivitePrincipaleEtablissement": false,
                    "CaractereEmployeurEtablissement": "N",
                    "IndCaractereEmployeurEtablissement": false,
                    "Enseigne1": null,
                    "Enseigne2": null,
                    "Enseigne3": null,
                    "IndEnseigneEtablissement": false
                }
            ]
        },
        {
            "Siren": "304536279",
            "Nic": "00017",
            "StatutDiffusionEtablissement": "O",
            "DateCreationEtablissement": null,
            "NombrePeriodes": 1,
            "UniteLegale": {
                "StatutDiffusionUniteLegale": "O",
                "DateCreationUniteLegale": "1900-01-01",
                "Sigle": null,
                "Sexe": 1,
                "NomUsage": null,
                "Prenom1": "LOUIS",
                "Prenom2": null,
                "Prenom3": null,
                "Prenom4": null,
                "PrenomUsuel": "LOUIS",
                "CaractereEmployeur": "N",
                "UnitePurgee": true,
                "EtatAdministratif": "C",
                "Nom": "GOUGELIN",
                "Denomination": null,
                "ActivitePrincipale": "69.23",
                "LibelleActivite": "Taxis",
                "NomenclatureActivite": "NAP",
                "CategorieJuridique": null,
                "CategorieProfessionnelle": "1000",
                "NICSiege": "00017"
            },
            "Adresse": {
                "ComplementAdresseEtablissement": null,
                "NumeroVoieEtablissement": "13",
                "IndiceRepetitionEtablissement": null,
                "TypeVoieEtablissement": "RUE",
                "LibelleVoieEtablissement": "ALFRED DE MUSSET",
                "CodePostalEtablissement": "92240",
                "LibelleCommuneEtablissement": "MALAKOFF",
                "LibelleCommuneEtrangerEtablissement": null,
                "DistributionSpecialeEtablissement": null,
                "CodeCommuneEtablissement": "92046",
                "CedexEtablissement": null
            },
            "Periodes": [
                {
                    "DateFin": null,
                    "DateDebut": "2000-07-10",
                    "EtatAdministratifEtablissement": "F",
                    "IndEtatAdministratifEtablissement": true,
                    "ActivitePrincipaleEtablissement": "69.23",
                    "LibelleActiviteEtablissement": "Taxis",
                    "NomenclatureActiviteEtablissement": "NAP",
                    "IndActivitePrincipaleEtablissement": false,
                    "CaractereEmployeurEtablissement": "N",
                    "IndCaractereEmployeurEtablissement": false,
                    "Enseigne1": null,
                    "Enseigne2": null,
                    "Enseigne3": null,
                    "IndEnseigneEtablissement": false
                }
            ]
        },
        {
            "Siren": "304967961",
            "Nic": "00018",
            "StatutDiffusionEtablissement": "O",
            "DateCreationEtablissement": null,
            "NombrePeriodes": 1,
            "UniteLegale": {
                "StatutDiffusionUniteLegale": "O",
                "DateCreationUniteLegale": "1900-01-01",
                "Sigle": null,
                "Sexe": 1,
                "NomUsage": null,
                "Prenom1": "ANDRE",
                "Prenom2": null,
                "Prenom3": null,
                "Prenom4": null,
                "PrenomUsuel": "ANDRE",
                "CaractereEmployeur": "N",
                "UnitePurgee": true,
                "EtatAdministratif": "C",
                "Nom": "GAUDEL",
                "Denomination": null,
                "ActivitePrincipale": "69.23",
                "LibelleActivite": "Taxis",
                "NomenclatureActivite": "NAP",
                "CategorieJuridique": null,
                "CategorieProfessionnelle": "1000",
                "NICSiege": "00018"
            },
            "Adresse": {
                "ComplementAdresseEtablissement": null,
                "NumeroVoieEtablissement": null,
                "IndiceRepetitionEtablissement": null,
                "TypeVoieEtablissement": "RUE",
                "LibelleVoieEtablissement": "GUY MOQUET",
                "CodePostalEtablissement": "92240",
                "LibelleCommuneEtablissement": "MALAKOFF",
                "LibelleCommuneEtrangerEtablissement": null,
                "DistributionSpecialeEtablissement": null,
                "CodeCommuneEtablissement": "92046",
                "CedexEtablissement": null
            },
            "Periodes": [
                {
                    "DateFin": null,
                    "DateDebut": "1985-12-25",
                    "EtatAdministratifEtablissement": "F",
                    "IndEtatAdministratifEtablissement": true,
                    "ActivitePrincipaleEtablissement": "69.23",
                    "LibelleActiviteEtablissement": "Taxis",
                    "NomenclatureActiviteEtablissement": "NAP",
                    "IndActivitePrincipaleEtablissement": false,
                    "CaractereEmployeurEtablissement": "N",
                    "IndCaractereEmployeurEtablissement": false,
                    "Enseigne1": null,
                    "Enseigne2": null,
                    "Enseigne3": null,
                    "IndEnseigneEtablissement": false
                }
            ]
        },
        {
            "Siren": "304445562",
            "Nic": "00024",
            "StatutDiffusionEtablissement": "O",
            "DateCreationEtablissement": null,
            "NombrePeriodes": 1,
            "UniteLegale": {
                "StatutDiffusionUniteLegale": "O",
                "DateCreationUniteLegale": "1975-12-25",
                "Sigle": null,
                "Sexe": 1,
                "NomUsage": null,
                "Prenom1": "ALBERT",
                "Prenom2": null,
                "Prenom3": null,
                "Prenom4": null,
                "PrenomUsuel": "ALBERT",
                "CaractereEmployeur": "N",
                "UnitePurgee": true,
                "EtatAdministratif": "C",
                "Nom": "CARTIER",
                "Denomination": null,
                "ActivitePrincipale": "52.4C",
                "LibelleActivite": "Commerce de détail d'habillement",
                "NomenclatureActivite": "NAFRev1",
                "CategorieJuridique": null,
                "CategorieProfessionnelle": "1000",
                "NICSiege": "00024"
            },
            "Adresse": {
                "ComplementAdresseEtablissement": null,
                "NumeroVoieEtablissement": "54",
                "IndiceRepetitionEtablissement": null,
                "TypeVoieEtablissement": "AV",
                "LibelleVoieEtablissement": "PIERRE LAROUSSE",
                "CodePostalEtablissement": "92240",
                "LibelleCommuneEtablissement": "MALAKOFF",
                "LibelleCommuneEtrangerEtablissement": null,
                "DistributionSpecialeEtablissement": null,
                "CodeCommuneEtablissement": "92046",
                "CedexEtablissement": null
            },
            "Periodes": [
                {
                    "DateFin": null,
                    "DateDebut": "1993-12-31",
                    "EtatAdministratifEtablissement": "F",
                    "IndEtatAdministratifEtablissement": true,
                    "ActivitePrincipaleEtablissement": "52.4C",
                    "LibelleActiviteEtablissement": "Commerce de détail d'habillement",
                    "NomenclatureActiviteEtablissement": "NAF1993",
                    "IndActivitePrincipaleEtablissement": false,
                    "CaractereEmployeurEtablissement": "N",
                    "IndCaractereEmployeurEtablissement": false,
                    "Enseigne1": null,
                    "Enseigne2": null,
                    "Enseigne3": null,
                    "IndEnseigneEtablissement": false
                }
            ]
        },
        {
            "Siren": "304850373",
            "Nic": "00032",
            "StatutDiffusionEtablissement": "O",
            "DateCreationEtablissement": "1900-01-01",
            "NombrePeriodes": 4,
            "UniteLegale": {
                "StatutDiffusionUniteLegale": "O",
                "DateCreationUniteLegale": "1900-01-01",
                "Sigle": "ERAAM",
                "Sexe": null,
                "NomUsage": null,
                "Prenom1": null,
                "Prenom2": null,
                "Prenom3": null,
                "Prenom4": null,
                "PrenomUsuel": null,
                "CaractereEmployeur": "O",
                "EtatAdministratif": "C",
                "Nom": null,
                "Denomination": "ETUDE RECHER APPLI AIDE MAINTENANCE SARL",
                "ActivitePrincipale": "73.1Z",
                "LibelleActivite": "Recherche-développement en sciences physiques et naturelles",
                "NomenclatureActivite": "NAFRev1",
                "CategorieJuridique": "5499",
                "CategorieProfessionnelle": null,
                "NICSiege": "00073"
            },
            "Adresse": {
                "ComplementAdresseEtablissement": null,
                "NumeroVoieEtablissement": "1",
                "IndiceRepetitionEtablissement": null,
                "TypeVoieEtablissement": "RUE",
                "LibelleVoieEtablissement": "DE LA TOUR",
                "CodePostalEtablissement": "92240",
                "LibelleCommuneEtablissement": "MALAKOFF",
                "LibelleCommuneEtrangerEtablissement": null,
                "DistributionSpecialeEtablissement": null,
                "CodeCommuneEtablissement": "92046",
                "CedexEtablissement": null
            },
            "Periodes": [
                {
                    "DateFin": null,
                    "DateDebut": "1995-12-25",
                    "EtatAdministratifEtablissement": "F",
                    "IndEtatAdministratifEtablissement": false,
                    "ActivitePrincipaleEtablissement": "74.3B",
                    "LibelleActiviteEtablissement": "Analyses, essais et inspections techniques",
                    "NomenclatureActiviteEtablissement": "NAF1993",
                    "IndActivitePrincipaleEtablissement": false,
                    "CaractereEmployeurEtablissement": "O",
                    "IndCaractereEmployeurEtablissement": true,
                    "Enseigne1": null,
                    "Enseigne2": null,
                    "Enseigne3": null,
                    "IndEnseigneEtablissement": false
                },
                {
                    "DateFin": "1995-12-24",
                    "DateDebut": "1995-05-01",
                    "EtatAdministratifEtablissement": "F",
                    "IndEtatAdministratifEtablissement": true,
                    "ActivitePrincipaleEtablissement": "74.3B",
                    "LibelleActiviteEtablissement": "Analyses, essais et inspections techniques",
                    "NomenclatureActiviteEtablissement": "NAF1993",
                    "IndActivitePrincipaleEtablissement": false,
                    "CaractereEmployeurEtablissement": null,
                    "IndCaractereEmployeurEtablissement": false,
                    "Enseigne1": null,
                    "Enseigne2": null,
                    "Enseigne3": null,
                    "IndEnseigneEtablissement": false
                },
                {
                    "DateFin": "1995-04-30",
                    "DateDebut": "1994-12-25",
                    "EtatAdministratifEtablissement": "A",
                    "IndEtatAdministratifEtablissement": false,
                    "ActivitePrincipaleEtablissement": "74.3B",
                    "LibelleActiviteEtablissement": "Analyses, essais et inspections techniques",
                    "NomenclatureActiviteEtablissement": "NAF1993",
                    "IndActivitePrincipaleEtablissement": true,
                    "CaractereEmployeurEtablissement": null,
                    "IndCaractereEmployeurEtablissement": false,
                    "Enseigne1": null,
                    "Enseigne2": null,
                    "Enseigne3": null,
                    "IndEnseigneEtablissement": false
                },
                {
                    "DateFin": "1994-12-24",
                    "DateDebut": "1900-01-01",
                    "EtatAdministratifEtablissement": "A",
                    "IndEtatAdministratifEtablissement": true,
                    "ActivitePrincipaleEtablissement": null,
                    "LibelleActiviteEtablissement": null,
                    "NomenclatureActiviteEtablissement": null,
                    "IndActivitePrincipaleEtablissement": true,
                    "CaractereEmployeurEtablissement": null,
                    "IndCaractereEmployeurEtablissement": true,
                    "Enseigne1": null,
                    "Enseigne2": null,
                    "Enseigne3": null,
                    "IndEnseigneEtablissement": true
                }
            ]
        },
        {
            "Siren": "306990565",
            "Nic": "00013",
            "StatutDiffusionEtablissement": "O",
            "DateCreationEtablissement": null,
            "NombrePeriodes": 1,
            "UniteLegale": {
                "StatutDiffusionUniteLegale": "O",
                "DateCreationUniteLegale": "1900-01-01",
                "Sigle": null,
                "Sexe": 2,
                "NomUsage": null,
                "Prenom1": "CHRISTIANE",
                "Prenom2": null,
                "Prenom3": null,
                "Prenom4": null,
                "PrenomUsuel": "CHRISTIANE",
                "CaractereEmployeur": "N",
                "UnitePurgee": true,
                "EtatAdministratif": "C",
                "Nom": "CARRE",
                "Denomination": null,
                "ActivitePrincipale": null,
                "LibelleActivite": null,
                "NomenclatureActivite": null,
                "CategorieJuridique": null,
                "CategorieProfessionnelle": "1000",
                "NICSiege": "00013"
            },
            "Adresse": {
                "ComplementAdresseEtablissement": null,
                "NumeroVoieEtablissement": null,
                "IndiceRepetitionEtablissement": null,
                "TypeVoieEtablissement": "RUE",
                "LibelleVoieEtablissement": "LOUIS GIRARD",
                "CodePostalEtablissement": "92240",
                "LibelleCommuneEtablissement": "MALAKOFF",
                "LibelleCommuneEtrangerEtablissement": null,
                "DistributionSpecialeEtablissement": null,
                "CodeCommuneEtablissement": "92046",
                "CedexEtablissement": null
            },
            "Periodes": [
                {
                    "DateFin": null,
                    "DateDebut": "1984-12-25",
                    "EtatAdministratifEtablissement": "F",
                    "IndEtatAdministratifEtablissement": true,
                    "ActivitePrincipaleEtablissement": null,
                    "LibelleActiviteEtablissement": null,
                    "NomenclatureActiviteEtablissement": null,
                    "IndActivitePrincipaleEtablissement": false,
                    "CaractereEmployeurEtablissement": "N",
                    "IndCaractereEmployeurEtablissement": false,
                    "Enseigne1": null,
                    "Enseigne2": null,
                    "Enseigne3": null,
                    "IndEnseigneEtablissement": false
                }
            ]
        },
        {
            "Siren": "307835256",
            "Nic": "00016",
            "StatutDiffusionEtablissement": "O",
            "DateCreationEtablissement": null,
            "NombrePeriodes": 1,
            "UniteLegale": {
                "StatutDiffusionUniteLegale": "O",
                "DateCreationUniteLegale": "1900-01-01",
                "Sigle": null,
                "Sexe": 1,
                "NomUsage": null,
                "Prenom1": "GERARD",
                "Prenom2": null,
                "Prenom3": null,
                "Prenom4": null,
                "PrenomUsuel": "GERARD",
                "CaractereEmployeur": "N",
                "UnitePurgee": true,
                "EtatAdministratif": "C",
                "Nom": "BENICHOU",
                "Denomination": null,
                "ActivitePrincipale": "60.2E",
                "LibelleActivite": "Transport de voyageurs par taxis",
                "NomenclatureActivite": "NAFRev1",
                "CategorieJuridique": null,
                "CategorieProfessionnelle": "1000",
                "NICSiege": "00016"
            },
            "Adresse": {
                "ComplementAdresseEtablissement": null,
                "NumeroVoieEtablissement": "60",
                "IndiceRepetitionEtablissement": null,
                "TypeVoieEtablissement": "AV",
                "LibelleVoieEtablissement": "AUGUSTIN DUMONT",
                "CodePostalEtablissement": "92240",
                "LibelleCommuneEtablissement": "MALAKOFF",
                "LibelleCommuneEtrangerEtablissement": null,
                "DistributionSpecialeEtablissement": null,
                "CodeCommuneEtablissement": "92046",
                "CedexEtablissement": null
            },
            "Periodes": [
                {
                    "DateFin": null,
                    "DateDebut": "1995-11-14",
                    "EtatAdministratifEtablissement": "F",
                    "IndEtatAdministratifEtablissement": true,
                    "ActivitePrincipaleEtablissement": "60.2E",
                    "LibelleActiviteEtablissement": "Transport de voyageurs par taxis",
                    "NomenclatureActiviteEtablissement": "NAF1993",
                    "IndActivitePrincipaleEtablissement": false,
                    "CaractereEmployeurEtablissement": "N",
                    "IndCaractereEmployeurEtablissement": false,
                    "Enseigne1": null,
                    "Enseigne2": null,
                    "Enseigne3": null,
                    "IndEnseigneEtablissement": false
                }
            ]
        },
        {
            "Siren": "308914829",
            "Nic": "00012",
            "StatutDiffusionEtablissement": "O",
            "DateCreationEtablissement": "1976-01-01",
            "NombrePeriodes": 4,
            "UniteLegale": {
                "StatutDiffusionUniteLegale": "O",
                "DateCreationUniteLegale": "1976-01-01",
                "Sigle": null,
                "Sexe": 1,
                "NomUsage": null,
                "Prenom1": "GUY",
                "Prenom2": null,
                "Prenom3": null,
                "Prenom4": null,
                "PrenomUsuel": "GUY",
                "CaractereEmployeur": "N",
                "EtatAdministratif": "A",
                "Nom": "HOCDE",
                "Denomination": null,
                "ActivitePrincipale": "68.20B",
                "LibelleActivite": "Location de terrains et d'autres biens immobiliers",
                "NomenclatureActivite": "NAFRev2",
                "CategorieJuridique": null,
                "CategorieProfessionnelle": "1000",
                "NICSiege": "00012"
            },
            "Adresse": {
                "ComplementAdresseEtablissement": null,
                "NumeroVoieEtablissement": "76",
                "IndiceRepetitionEtablissement": null,
                "TypeVoieEtablissement": "RUE",
                "LibelleVoieEtablissement": "HOCHE",
                "CodePostalEtablissement": "92240",
                "LibelleCommuneEtablissement": "MALAKOFF",
                "LibelleCommuneEtrangerEtablissement": null,
                "DistributionSpecialeEtablissement": null,
                "CodeCommuneEtablissement": "92046",
                "CedexEtablissement": null
            },
            "Periodes": [
                {
                    "DateFin": null,
                    "DateDebut": "2009-12-25",
                    "EtatAdministratifEtablissement": "F",
                    "IndEtatAdministratifEtablissement": true,
                    "ActivitePrincipaleEtablissement": "68.20B",
                    "LibelleActiviteEtablissement": "Location de terrains et d'autres biens immobiliers",
                    "NomenclatureActiviteEtablissement": "NAFRev2",
                    "IndActivitePrincipaleEtablissement": false,
                    "CaractereEmployeurEtablissement": "N",
                    "IndCaractereEmployeurEtablissement": false,
                    "Enseigne1": null,
                    "Enseigne2": null,
                    "Enseigne3": null,
                    "IndEnseigneEtablissement": false
                },
                {
                    "DateFin": "2009-12-24",
                    "DateDebut": "2008-01-01",
                    "EtatAdministratifEtablissement": "A",
                    "IndEtatAdministratifEtablissement": false,
                    "ActivitePrincipaleEtablissement": "68.20B",
                    "LibelleActiviteEtablissement": "Location de terrains et d'autres biens immobiliers",
                    "NomenclatureActiviteEtablissement": "NAFRev2",
                    "IndActivitePrincipaleEtablissement": true,
                    "CaractereEmployeurEtablissement": "N",
                    "IndCaractereEmployeurEtablissement": false,
                    "Enseigne1": null,
                    "Enseigne2": null,
                    "Enseigne3": null,
                    "IndEnseigneEtablissement": false
                },
                {
                    "DateFin": "2007-12-31",
                    "DateDebut": "1987-12-25",
                    "EtatAdministratifEtablissement": "A",
                    "IndEtatAdministratifEtablissement": false,
                    "ActivitePrincipaleEtablissement": "70.2C",
                    "LibelleActiviteEtablissement": "Location d'autres biens immobiliers",
                    "NomenclatureActiviteEtablissement": "NAF1993",
                    "IndActivitePrincipaleEtablissement": true,
                    "CaractereEmployeurEtablissement": "N",
                    "IndCaractereEmployeurEtablissement": false,
                    "Enseigne1": null,
                    "Enseigne2": null,
                    "Enseigne3": null,
                    "IndEnseigneEtablissement": false
                },
                {
                    "DateFin": "1987-12-24",
                    "DateDebut": "1976-01-01",
                    "EtatAdministratifEtablissement": "A",
                    "IndEtatAdministratifEtablissement": true,
                    "ActivitePrincipaleEtablissement": null,
                    "LibelleActiviteEtablissement": null,
                    "NomenclatureActiviteEtablissement": null,
                    "IndActivitePrincipaleEtablissement": true,
                    "CaractereEmployeurEtablissement": "N",
                    "IndCaractereEmployeurEtablissement": true,
                    "Enseigne1": null,
                    "Enseigne2": null,
                    "Enseigne3": null,
                    "IndEnseigneEtablissement": true
                }
            ]
        }
    ]
}
```





<!-- .slide: class="slide" -->
### Recherche sur une variable historisée
**Syntaxe** : periode(nomVariable:valeur)

La recherche se fait par défaut sur tout l'historique, sinon il faut préciser un paramètre date.

 - toutes les unités légales dont la dénomination contient ou a contenu le mot GAZ
 ```
 /ws/siren?q=periode(Denomination:GAZ)
 ```
 - tous les établissements dont l'activité principale a été la construction de cellules d'aéronefs
```
/ws/siret?q=periode(ActivitePrincipaleEtablissement:33.01)
```





<!-- .slide: class="slide" -->
### Recherche par élimination
**Syntaxe** : -nomVariable:valeur ou -periode(nomVariable:valeur)

 - tous les établissements qui n'ont jamais été fermés
```
/ws/siret?q=-periode(EtatAdministratifEtablissement:F)
```





<!-- .slide: class="slide" -->
### Recherche sur plusieurs variables
**Syntaxe** : nomVariable1:valeur1 *AND/OR* nomVariable2:valeur2

 - toutes les entreprises dont l'activité principale a été au moins à un moment donné 56.10A (restauration traditionnelle) ou 56.10C (restauration rapide)
```
/ws/siret?q=periode(ActivitePrincipale:56.10A OR ActivitePrincipale:56.10C)
```
 - tous les établissements sur la commune de Malakoff dont la dernière catégorie juridique de l'unité légale est 9220 (association déclarée)
```
/ws/siret?q=CodeCommuneEtablissement:92046 AND CategorieJuridique:9220
```





<!-- .slide: class="slide" -->
### Recherche à une date donnée
**Syntaxe** : periode(nomVariable:valeur)*&*date=AAAA-MM-JJ

Cela renvoie malgré tout l'intégralité de l'historique.

 - toutes les unités légales actives au 18/09/2009
```
/ws/siren?q=periode(EtatAdministratif:A)&date=2009-09-18
```
 - tous les établissements de Malakoff faisant principalement de la restauration traditionnelle et actifs au 18/09/2009
```
/ws/siret?q=CodeCommuneEtablissement:92046 AND periode(EtatAdministratifEtablissement:A AND ActivitePrincipaleEtablissement:56.10A)&date=2009-09-18
```





<!-- .slide: class="slide" -->
### Recherche exacte
**Syntaxe** : nomVariable:"valeur"

 - toutes les unités légales actives au 03/12/2010 ayant la dénomination précise *LE VERRE GALANT*
```
/ws/siren?q=periode(Denomination:"LE VERRE GALANT" AND EtatAdministratif:A)&date=2010-12-03
```





<!-- .slide: class="slide" -->
### Utilisation de caractères spéciaux
**\*** : permet de remplacer une chaîne de caractères
```
/ws/siret?q=ActivitePrincipale:8*
```
**?** : permet de remplacer exactement un caractère
```
/ws/siret?q=Sigle:SNC?
```
**~** : permet de faire une recherche approximative au sens de Damerau-Levenshtein (soit 1 suppression/ajout/permutation, soit 2, par défaut)
```
/ws/siret?q=Prenom1:FLORENT~ AND -Prenom1:FLORENT
```





<!-- .slide: class="slide" -->
### Recherche avec une plage de valeurs
**Syntaxe** : nomVariable:[valeur1 TO valeur2]  (bornes incluses) 
**Syntaxe** : nomVariable:{valeur1 TO valeur2}  (bornes excluses)
              
Attention à utiliser l'encodage URL pour { (%7B) et } (%7D)

- Recherche des unités légales faisant principalement de la culture agricole au 01/09/2016
```
/ws/siren?q=periode(ActivitePrincipale:[01.1 TO 01.3} AND NomenclatureActivite:NAFRev2)&date=2016-09-01
```



