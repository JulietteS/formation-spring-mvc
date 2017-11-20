<!-- .slide: data-background-image="images/spring.png" data-background-size="1200px" class="chapter" -->
## 1
### API Sirene : recherche sur les unités légales

<!-- .slide: class="slide" -->
### Présentation du service
Obtenir les informations du répertoire sur une unité légale, identifiée par son <span style="color:red">siren</span>
 - l'historique complet (sur dénomination, nom de naissance, catégorie juridique, état, nic du siège, activité principale)
 - l'état à une date donnée
 - l'état courant (à la date de la base)

<!-- .slide: class="slide" -->
### Appel au service

GET /ws/siren/{siren}
GET /ws/siren/{siren}?date={date}
| Paramètre               | Description | Type de paramètre | Type  | Obligatoire                              |
| ----------------------- | ---------------------------------------------------------------------------------- |
| `siren`          | Numéro siren de l'entreprise (9 chiffres) | Path | String | Oui |
| `date`          | Date à laquelle on souhaite connaître l'état (AAAA-MM-JJ) | Query | String | Non |
| `Insee-source`| Information sur l'appelant. Doit être valorisé sous la forme Organisme:{Organisme},Application:{Application}|Header|String| Oui |
| `Accept`| Format de la réponse demandé (par défaut Application/json), demander Text/csv pour du CSV |Header|String| Non |
 
<!-- .slide: class="slide" -->
### Codes retour

| Code HTTP             | Résumé | Raison                               |
| ----------------------- | ---------------------------------------------------------------------------------- |
| `200`          | OK | Entreprise trouvée |
| `400`          | Bad Request | Paramètres incorrects ou manquants |
| `401`          | Unauthorized | Tentative de connection avec une adresse IP non autorisée |
| `403`          | Forbidden | Droits insuffisants pour accéder à cette unité |
| `404`          | Not Found | Unité non trouvée (siren inexistant ou pas encore créé à la date demandée) |
| `406`          | Not acceptable | Format demandé non prévu |

<!-- .slide: class="slide" -->
### Beans et injection des dépendances
Par annotation, version `@Autowired`
```java
@Repository
public class AdresseDaoImpl implements AdresseDao {
```
```java
@Service
public class AdresseServiceImpl implements AdresseService {

@Autowired
private AdresseDao adresseDao;
```
Par annotation, version `@Resource`
```java
@Repository("adresseDao1")
public class AdresseDaoImpl implements AdresseDao {
```
```java
@Service
public class AdresseServiceImpl implements AdresseService {

@Resource(name = "adresseDao1")
private AdresseDao adresseDao;
```





<!-- .slide: class="slide" -->
### Activer la détection des annotations
```xml
<context:component-scan base-package="fr.insee" />
```





<!-- .slide: class="slide" -->
### Injection d’une source de propriétés
Pour externaliser des propriétés non surchargeables par le C.E.I.
<small>Sinon, utiliser `InseeConfig`</small>
```
prefix.key.a=Valeur A
prefix.key.b=Valeur B
```
```java
@Component
@PropertySource("classpath:application.properties")
public class ComponentImpl {

@Value("${prefix.key.a}")
private String a;
```
