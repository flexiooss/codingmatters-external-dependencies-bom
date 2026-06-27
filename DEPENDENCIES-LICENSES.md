# Licences des dépendances du BOM

> Document généré à partir de `pom.xml` (`codingmatters-external-dependencies-bom` v1.67.0-SNAPSHOT).
> Il recense les dépendances déclarées dans `<dependencyManagement>`, leur licence,
> et vérifie le caractère **open source** de chacune.
>
> Date : 2026-06-27

## Synthèse

| Famille de licence | Open source | Type | Nb d'artefacts |
|--------------------|:-----------:|------|:--------------:|
| Apache License 2.0 | ✅ | Permissive | 33 |
| MIT | ✅ | Permissive | 5 |
| BSD (2/3-Clause) | ✅ | Permissive | 4 |
| Bouncy Castle (MIT-style) | ✅ | Permissive | 1 |
| HSQLDB License (BSD-style) | ✅ | Permissive | 1 |
| Java HTML Tidy License (zlib/MIT-style) | ✅ | Permissive | 1 |
| Unicode / ICU License | ✅ | Permissive | 1 |
| Eclipse Public License (EPL 1.0 / 2.0) | ✅ | Copyleft faible | 2 |
| EPL 1.0 / LGPL 2.1 (double licence) | ✅ | Copyleft faible | 4 |
| Jakarta Mail (EPL 2.0 / GPL2+CPE / EDL) | ✅ | Copyleft faible | 1 |
| LGPL (2.1 / 3.0) | ✅ | Copyleft | 4 |
| LGPL 2.1 / MPL 2.0 (double licence) | ✅ | Copyleft | 1 |
| **Gatling Highcharts License** | ❌ | **Propriétaire** | 1 |

### ⚠️ Points d'attention

- **`io.gatling.highcharts:gatling-charts-highcharts`** — **NON open source**. Licence
  propriétaire « Gatling Highcharts » : le module embarque Highcharts/Highstock (licence
  commerciale). Gatling le distribue gratuitement mais ne peut pas l'open-sourcer. Utilisé
  en `scope=test` ici, mais à ne **jamais** redistribuer dans un livrable.
- **PlantUML** — la variante **MIT** (`plantuml-mit`, 1.2026.6) est désormais utilisée, en
  remplacement de l'artefact `plantuml` qui était sous GPL. La variante MIT n'existant pas
  avant la 1.2023.x, le passage a impliqué une montée de version (depuis 1.2019.13).
- **Dépendances LGPL** (MariaDB connector, CSSBox, Flying Saucer, OpenPDF, Logback) :
  open source mais copyleft « faible ». Utilisables sans contaminer le code applicatif
  tant qu'elles restent en bibliothèques liées dynamiquement et non modifiées.

---

## Apache License 2.0 — ✅ permissive

Licence permissive standard, compatible avec un usage propriétaire.

| GroupId:ArtifactId | Version |
|--------------------|---------|
| com.fasterxml.jackson:jackson-bom | 2.20.0 |
| com.squareup:javapoet | 1.11.1 |
| org.raml:raml-parser-2 | 1.0.47 |
| org.apache.maven:maven-plugin-api | 3.9.9 |
| org.apache.maven:maven-core | 3.9.9 |
| org.apache.maven:maven-artifact | 3.9.9 |
| org.apache.maven:maven-compat | 3.9.9 |
| org.apache.maven.plugin-tools:maven-plugin-annotations | 3.15.1 |
| org.apache.maven.plugin-testing:maven-plugin-testing-harness | 4.0.0-beta-3 |
| io.undertow:undertow-core | 2.3.23.Final |
| io.undertow:undertow-servlet | 2.3.23.Final |
| com.squareup.okhttp3:okhttp | 5.1.0 |
| com.squareup.okhttp3:okhttp-jvm | 5.1.0 |
| org.apache.tinkerpop:tinkergraph-gremlin | 3.7.4 |
| org.apache.tinkerpop:gremlin-driver | 3.7.4 |
| org.mongodb:mongodb-driver-sync | 5.6.0 |
| org.mongodb:mongodb-driver-core | 5.6.0 |
| org.mongodb:bson | 5.6.0 |
| io.dropwizard.metrics:metrics-core | 4.2.37 |
| io.dropwizard.metrics:metrics-jvm | 4.2.37 |
| com.github.heremaps:oksse | 0.9.0 |
| commons-io:commons-io | 2.20.0 |
| org.apache.commons:commons-csv | 1.14.1 |
| org.apache.commons:commons-lang3 | 3.18.0 |
| commons-net:commons-net | 3.12.0 |
| org.apache.commons:commons-text | 1.14.0 |
| org.apache.pdfbox:pdfbox | 3.0.5 |
| org.apache.pdfbox:pdfbox-io | 3.0.5 |
| org.apache.poi:poi | 5.4.1 |
| org.apache.poi:poi-ooxml | 5.4.1 |
| xml-apis:xml-apis | 1.4.01 |
| org.shredzone.acme4j:acme4j-client | 3.5.1 |
| com.intuit.quickbooks-online:oauth2-platform-api | 5.0.3 |
| com.intuit.quickbooks-online:ipp-v3-java-devkit | 5.0.3 |
| com.intuit.quickbooks-online:ipp-v3-java-data | 5.0.3 |
| org.keycloak:keycloak-parent | 26.3.4 |
| com.jayway.jsonpath:json-path | 2.9.0 |
| net.minidev:json-smart | 2.6.0 |
| io.gatling:gatling-core-java | 3.14.4 |
| io.gatling:gatling-http-java | 3.14.4 |
| io.opentelemetry.instrumentation:opentelemetry-instrumentation-annotations | 2.25.0 |
| io.opentelemetry.javaagent:opentelemetry-javaagent | 2.25.0 |
| io.opentelemetry:opentelemetry-api | 1.59.0 |
| com.microsoft.playwright:playwright | 1.58.0 |

> Note : `xml-apis` est déclaré sous Apache 2.0 dans son POM, certains fichiers d'origine
> étant aussi sous W3C/DOM/SAX (domaine public). Permissif dans tous les cas.

## MIT License — ✅ permissive

| GroupId:ArtifactId | Version |
|--------------------|---------|
| org.slf4j:slf4j-api | 2.0.17 |
| org.slf4j:slf4j-simple | 2.0.17 |
| org.jsoup:jsoup | 1.21.2 |
| com.auth0:java-jwt | 4.5.0 |
| redis.clients:jedis | 6.2.0 |
| net.sourceforge.plantuml:plantuml-mit | 1.2026.6 |

## BSD (2 / 3-Clause) — ✅ permissive

| GroupId:ArtifactId | Version | Variante |
|--------------------|---------|----------|
| org.hamcrest:hamcrest | 3.0 | BSD 3-Clause |
| org.antlr:antlr4-runtime | 4.13.2 | BSD 3-Clause |
| org.commonmark:commonmark | 0.26.0 | BSD 2-Clause |
| com.github.mwiede:jsch | 2.27.3 | BSD (fork de JCraft JSch) |

## Bouncy Castle License — ✅ permissive

Adaptation de la licence MIT.

| GroupId:ArtifactId | Version |
|--------------------|---------|
| org.bouncycastle:bcprov-jdk18on | 1.82 |

## HSQLDB License — ✅ permissive

Licence de type BSD propre au projet HSQLDB.

| GroupId:ArtifactId | Version |
|--------------------|---------|
| org.hsqldb:hsqldb | 2.7.0 |

## Java HTML Tidy License — ✅ permissive

Licence de type zlib/MIT (W3C/MIT/INRIA/Keio), compatible usage propriétaire.

| GroupId:ArtifactId | Version |
|--------------------|---------|
| net.sf.jtidy:jtidy | r938 |

## Unicode / ICU License — ✅ permissive

Licence permissive type X/MIT (Unicode License).

| GroupId:ArtifactId | Version |
|--------------------|---------|
| com.ibm.icu:icu4j | 77.1 |

## Eclipse Public License (EPL) — ✅ copyleft faible

| GroupId:ArtifactId | Version | Licence |
|--------------------|---------|---------|
| junit:junit | 4.13.2 | EPL 1.0 |
| org.junit:junit-bom | 5.12.1 | EPL 2.0 |

## EPL 1.0 / LGPL 2.1 (double licence) — ✅ copyleft faible

Logback est distribué au choix sous EPL 1.0 ou LGPL 2.1.

| GroupId:ArtifactId | Version |
|--------------------|---------|
| ch.qos.logback:logback-core | 1.5.18 |
| ch.qos.logback:logback-classic | 1.5.18 |
| ch.qos.logback.contrib:logback-json-classic | 0.1.5 |
| ch.qos.logback.contrib:logback-jackson | 0.1.5 |

## Jakarta Mail — ✅ copyleft faible

Triple licence : EPL 2.0 / GPL 2.0 + Classpath Exception / EDL 1.0 (BSD-3).

| GroupId:ArtifactId | Version |
|--------------------|---------|
| com.sun.mail:jakarta.mail | 2.0.2 |

## LGPL (2.1 / 3.0) — ✅ copyleft

Open source ; copyleft « faible » : pas de contamination du code applicatif si la
bibliothèque est liée et non modifiée.

| GroupId:ArtifactId | Version | Licence |
|--------------------|---------|---------|
| org.xhtmlrenderer:flying-saucer-pdf-openpdf | 10.0.0 | LGPL 2.1 |
| org.xhtmlrenderer:flying-saucer-core | 10.0.0 | LGPL 2.1 |
| net.sf.cssbox:cssbox | 5.0.2 | LGPL 3.0 |
| org.mariadb.jdbc:mariadb-java-client | 2.7.12 | LGPL 2.1 |

## LGPL 2.1 / MPL 2.0 (double licence) — ✅ copyleft

| GroupId:ArtifactId | Version |
|--------------------|---------|
| com.github.librepdf:openpdf | 3.0.0 |

## Gatling Highcharts License — ❌ PROPRIÉTAIRE (non open source)

| GroupId:ArtifactId | Version | Remarque |
|--------------------|---------|----------|
| io.gatling.highcharts:gatling-charts-highcharts | 3.14.4 | Licence propriétaire, embarque Highcharts/Highstock (commercial). Distribué gratuitement par Gatling. Ici en `scope=test`. **Ne pas redistribuer.** |

---

## Notes méthodologiques

- Seules les dépendances de `<dependencyManagement>` sont couvertes (cœur du BOM). Les
  plugins Maven du bloc `<build>` (presque tous Apache 2.0) ne sont pas listés.
- Les licences ont été établies à partir des POM publiés sur Maven Central et des dépôts
  d'origine. Les cas non triviaux ont été vérifiés en ligne :
  - Gatling Highcharts : <https://central.sonatype.com/artifact/io.gatling.highcharts/gatling-charts-highcharts> — confirmé propriétaire.
  - PlantUML : <https://central.sonatype.com/artifact/net.sourceforge.plantuml/plantuml-mit> — variante MIT (l'artefact `plantuml` étant sous GPL).
  - MariaDB Connector/J : <https://github.com/mariadb-corporation/mariadb-connector-j> — LGPL 2.1.
  - JTidy : <https://jtidy.sourceforge.net/license.html> — Java HTML Tidy License.
  - oksse : <https://github.com/heremaps/oksse/blob/master/LICENSE> — Apache 2.0.
- « Open source » = licence approuvée OSI / FSF. Le **copyleft** (GPL/LGPL/EPL/MPL)
  reste open source mais impose des obligations de redistribution à connaître.
