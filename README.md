## Valider la qualité du code avec Checkstyle
**Quelle est la norme de codage à laquelle se réfère le rapport par défaut ?**

sun_checks.xml - Sun Microsystems Definition (default). (https://maven.apache.org/plugins/maven-checkstyle-plugin/examples/custom-checker-config.html)

**Comment imposer la norme de codage de Google?**

```xml
<configuration>
  <configLocation>google_checks.xml</configLocation>
</configuration>
```

## Rapport croisé de source
**Quelle est la valeur ajoutée de ce plugin ?**

Il permet de faire le lien entre un numéro de ligne de code et cette ligne directement

**En particulier, montrez sa complémentarité avec CheckStyle. Désormais vous pouvez passer du rapport CheckStyle au code source en cliquant sur le numéro de ligne associé au commentaire CheckStyle.**

Il est possible d'acceder à la ligne où on a une erreur CheckStyle via un lien.


## Couverture des tests avec JaCoCo
**A quel point les développeurs ont réalisé des tests unitaires ?**
Il n'y en a aucun.

**Quelles parties de l'application n'ont pas été testées ?**
Toutes les classes.

**Ecrivez quelques tests en JUnit (/tpmaven/src/test/java/fr/esir/omd/ci/tpmaven/FirstPdfTest.java), et voyez quelle couverture de code vous obtenez.**
On obtient une couverture de 98%% pour la classe FirstPdf et 0% pour la classe App.

## Identifier des patterns d'erreur avec PMD

CPD:	Duplicate code detection.

PMD:	Verification of coding rules.
see https://pmd.sourceforge.io/pmd-6.50.0/pmd_rules_java.html

## Connaître l'activité du projet