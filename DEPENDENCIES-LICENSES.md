# Licences des dépendances du BOM

> Document généré à partir de `pom.xml` (`codingmatters-external-dependencies-bom` v1.67.0-SNAPSHOT).
> Il recense les licences des dépendances et vérifie le caractère **open source** de chacune.
>
> Deux parties :
> 1. **Dépendances directes** — déclarées dans `<dependencyManagement>` du BOM.
> 2. **[Dépendances transitives](#dépendances-transitives-clôture-complète)** — clôture
>    complète résolue par Maven (305 artefacts).
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
  commerciale). Gatling le distribue gratuitement mais ne peut pas l'open-sourcer.
  **Mitigation** : non redistribuée — utilisée uniquement en `scope=test` pour les tests
  en charge sur l'application Flexio.
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
| io.gatling.highcharts:gatling-charts-highcharts | 3.14.4 | Licence propriétaire, embarque Highcharts/Highstock (commercial). Distribué gratuitement par Gatling. Ici en `scope=test`. **Non redistribuée.** |

> **Mitigation** : cette dépendance n'est pas distribuée. Elle est utilisée uniquement pour
> réaliser des tests en charge sur l'application Flexio.

## Dépendances transitives (clôture complète)

> Arbre de dépendances résolu par Maven à partir d'un POM de travail important le BOM
> et déclarant toutes ses dépendances. **305 artefacts** au total (directs + transitifs).
> Licences extraites automatiquement des POM via `license-maven-plugin`.

### Synthèse par licence (clôture transitive)

| Famille de licence | Open source | Type | Nb |
|--------------------|:-----------:|------|:--:|
| Apache License 2.0 | ✅ | Permissive | 224 |
| BSD (2/3-Clause / style) | ✅ | Permissive | 16 |
| MIT | ✅ | Permissive | 14 |
| EPL (Eclipse, copyleft faible) | ✅ | Copyleft faible | 13 |
| LGPL (copyleft) | ✅ | Copyleft | 8 |
| Apache-2.0 OU LGPL (double licence) | ✅ | Copyleft (choix Apache) | 6 |
| EPL / LGPL (double licence) | ✅ | Copyleft faible | 5 |
| Bouncy Castle (MIT-style) | ✅ | Permissive | 4 |
| CDDL / GPL (double licence) | ✅ | Copyleft faible (choix CDDL) | 4 |
| MPL (Mozilla, copyleft faible) | ✅ | Copyleft faible | 3 |
| EDL 1.0 (BSD-style) | ✅ | Permissive | 2 |
| CDDL | ✅ | Copyleft faible | 1 |
| Domaine public | ✅ | Domaine public | 1 |
| Gatling Highcharts (PROPRIÉTAIRE) | ❌ | Propriétaire | 1 |
| Java HTML Tidy (zlib/MIT-style) | ✅ | Permissive | 1 |
| The JSON License (non-OSI) | ❌ | Non-OSI | 1 |
| Unicode (permissive) | ✅ | Permissive | 1 |
| **TOTAL** | | | **305** |

### ⚠️ Points d'attention sur les transitives

- **`org.json:json:20160810`** — *The JSON License* (clause « *The Software shall be used for Good, not Evil* »). **Non reconnue open source** par l'OSI/FSF et explicitement bannie par Apache (catégorie X). Tirée transitivement par le SDK QuickBooks (`com.intuit.quickbooks-online:oauth2-platform-api`). Voir l'[analyse d'impact détaillée](#analyse-dimpact--orgjson-the-json-license) : exposition pratique quasi nulle (QuickBooks abandonné/non déployé, import mort côté backend).
- **`io.gatling.highcharts:gatling-charts-highcharts`** — propriétaire (cf. section dédiée). Non redistribuée, usage tests de charge uniquement.
- **LGPL** (copyleft) tirées transitivement : `openpdf`, `cssbox`, `jstyleparser`, `mariadb-java-client`, `flying-saucer-core`/`-pdf`, `spotbugs-annotations`, `com.google.code.findbugs:annotations`. Sans impact tant qu'elles restent liées et non modifiées.
- **CDDL / GPLv2** (double licence) : `com.sun.mail:javax.mail:1.6.1`, `javax.json:javax.json-api`, `org.glassfish:javax.json`, `javax.xml.bind:jaxb-api`. Double licence → on retient CDDL (permissive). À noter : `javax.mail:1.6.1` fait doublon avec `jakarta.mail:2.0.2` (ancien JavaMail tiré transitivement).
- **Apache 2.0 OU LGPLv3** (double licence) : modules `com.github.fge:*` et `com.github.java-json-tools:*` → on retient Apache 2.0.
- **MPL 2.0 / 1.1** (copyleft faible) : `Saxon-HE`, `org.mozilla:rhino`, `juniversalchardet`.

### Détail par licence

<details><summary><strong>Apache License 2.0</strong> — ✅ Permissive (224)</summary>

- `cglib:cglib:2.2.2`
- `com.aayushatharva.brotli4j:brotli4j:1.16.0`
- `com.aayushatharva.brotli4j:native-linux-aarch64:1.16.0`
- `com.aayushatharva.brotli4j:native-linux-x86_64:1.16.0`
- `com.aayushatharva.brotli4j:native-osx-aarch64:1.16.0`
- `com.aayushatharva.brotli4j:native-osx-x86_64:1.16.0`
- `com.aayushatharva.brotli4j:native-windows-x86_64:1.16.0`
- `com.aayushatharva.brotli4j:service:1.16.0`
- `com.carrotsearch:hppc:0.7.1`
- `com.fasterxml.jackson.core:jackson-annotations:2.20`
- `com.fasterxml.jackson.core:jackson-core:2.20.0`
- `com.fasterxml.jackson.core:jackson-databind:2.20.0`
- `com.fasterxml.jackson.datatype:jackson-datatype-jdk8:2.20.0`
- `com.fasterxml.jackson.datatype:jackson-datatype-jsr310:2.20.0`
- `com.fasterxml.jackson.jaxrs:jackson-jaxrs-base:2.20.0`
- `com.fasterxml.jackson.jaxrs:jackson-jaxrs-json-provider:2.20.0`
- `com.fasterxml.jackson.module:jackson-module-jaxb-annotations:2.20.0`
- `com.fasterxml.jackson.module:jackson-module-jsonSchema:2.20.0`
- `com.fasterxml.woodstox:woodstox-core:7.1.0`
- `com.github.ben-manes.caffeine:caffeine:3.2.0`
- `com.github.heremaps:oksse:0.9.0`
- `com.google.code.findbugs:jsr305:3.0.2`
- `com.google.code.gson:gson:2.12.1`
- `com.google.errorprone:error_prone_annotations:2.36.0`
- `com.google.guava:failureaccess:1.0.1`
- `com.google.guava:guava:33.4.0-jre`
- `com.google.inject:guice:5.1.0`
- `com.googlecode.libphonenumber:libphonenumber:8.0.0`
- `com.intuit.quickbooks-online:ipp-v3-java-data:5.0.3`
- `com.intuit.quickbooks-online:ipp-v3-java-devkit:5.0.3`
- `com.intuit.quickbooks-online:oauth2-platform-api:5.0.3`
- `com.jayway.jsonpath:json-path:2.9.0`
- `com.microsoft.playwright:driver-bundle:1.58.0`
- `com.microsoft.playwright:driver:1.58.0`
- `com.microsoft.playwright:playwright:1.58.0`
- `com.squareup.okhttp3:okhttp-jvm:5.1.0`
- `com.squareup.okhttp3:okhttp:5.1.0`
- `com.squareup.okio:okio-jvm:3.15.0`
- `com.squareup.okio:okio:3.15.0`
- `com.squareup:javapoet:1.11.1`
- `com.tdunning:t-digest:3.3`
- `com.typesafe.scala-logging:scala-logging_2.13:3.9.5`
- `com.typesafe:config:1.4.5`
- `com.zaxxer:SparseBitSet:1.3`
- `commons-beanutils:commons-beanutils-core:1.8.0`
- `commons-beanutils:commons-beanutils:1.9.4`
- `commons-codec:commons-codec:1.18.0`
- `commons-collections:commons-collections:3.2.2`
- `commons-configuration:commons-configuration:1.6`
- `commons-digester:commons-digester:1.8`
- `commons-io:commons-io:2.20.0`
- `commons-lang:commons-lang:2.6`
- `commons-logging:commons-logging:1.3.5`
- `commons-net:commons-net:3.12.0`
- `io.dropwizard.metrics:metrics-core:4.2.37`
- `io.dropwizard.metrics:metrics-jvm:4.2.37`
- `io.gatling:gatling-app:3.14.4`
- `io.gatling:gatling-charts:3.14.4`
- `io.gatling:gatling-commons:3.14.4`
- `io.gatling:gatling-core-java:3.14.4`
- `io.gatling:gatling-core:3.14.4`
- `io.gatling:gatling-http-client:3.14.4`
- `io.gatling:gatling-http-java:3.14.4`
- `io.gatling:gatling-http:3.14.4`
- `io.gatling:gatling-jdbc-java:3.14.4`
- `io.gatling:gatling-jdbc:3.14.4`
- `io.gatling:gatling-jms-java:3.14.4`
- `io.gatling:gatling-jms:3.14.4`
- `io.gatling:gatling-jsonpath:3.14.4`
- `io.gatling:gatling-netty-util:3.14.4`
- `io.gatling:gatling-quicklens:3.14.4`
- `io.gatling:gatling-recorder:3.14.4`
- `io.gatling:gatling-redis-java:3.14.4`
- `io.gatling:gatling-redis:3.14.4`
- `io.gatling:gatling-shared-cli:0.0.6`
- `io.gatling:gatling-shared-model_2.13:0.1.1`
- `io.gatling:gatling-shared-util_2.13:0.0.12`
- `io.github.metarank:cfor_2.13:0.3`
- `io.netty:netty-all:4.1.124.Final`
- `io.netty:netty-buffer:4.1.124.Final`
- `io.netty:netty-codec-dns:4.1.124.Final`
- `io.netty:netty-codec-haproxy:4.1.124.Final`
- `io.netty:netty-codec-http2:4.1.124.Final`
- `io.netty:netty-codec-http:4.1.124.Final`
- `io.netty:netty-codec-memcache:4.1.124.Final`
- `io.netty:netty-codec-mqtt:4.1.124.Final`
- `io.netty:netty-codec-redis:4.1.124.Final`
- `io.netty:netty-codec-smtp:4.1.124.Final`
- `io.netty:netty-codec-socks:4.1.124.Final`
- `io.netty:netty-codec-stomp:4.1.124.Final`
- `io.netty:netty-codec-xml:4.1.124.Final`
- `io.netty:netty-codec:4.1.124.Final`
- `io.netty:netty-common:4.1.124.Final`
- `io.netty:netty-handler-proxy:4.1.124.Final`
- `io.netty:netty-handler-ssl-ocsp:4.1.124.Final`
- `io.netty:netty-handler:4.1.124.Final`
- `io.netty:netty-resolver-dns-classes-macos:4.1.124.Final`
- `io.netty:netty-resolver-dns-native-macos:4.1.124.Final`
- `io.netty:netty-resolver-dns:4.1.124.Final`
- `io.netty:netty-resolver:4.1.124.Final`
- `io.netty:netty-tcnative-boringssl-static:2.0.72.Final`
- `io.netty:netty-tcnative-classes:2.0.72.Final`
- `io.netty:netty-transport-classes-epoll:4.1.124.Final`
- `io.netty:netty-transport-classes-io_uring:4.2.6.Final`
- `io.netty:netty-transport-classes-kqueue:4.1.124.Final`
- `io.netty:netty-transport-native-epoll:4.1.124.Final`
- `io.netty:netty-transport-native-io_uring:4.2.6.Final`
- `io.netty:netty-transport-native-kqueue:4.1.124.Final`
- `io.netty:netty-transport-native-unix-common:4.1.124.Final`
- `io.netty:netty-transport-rxtx:4.1.124.Final`
- `io.netty:netty-transport-sctp:4.1.124.Final`
- `io.netty:netty-transport-udt:4.1.124.Final`
- `io.netty:netty-transport:4.1.124.Final`
- `io.opentelemetry.instrumentation:opentelemetry-instrumentation-annotations:2.25.0`
- `io.opentelemetry:opentelemetry-api:1.59.0`
- `io.opentelemetry:opentelemetry-context:1.44.1`
- `io.smallrye.common:smallrye-common-annotation:2.12.0`
- `io.smallrye.common:smallrye-common-constraint:2.12.0`
- `io.smallrye.common:smallrye-common-cpu:2.12.0`
- `io.smallrye.common:smallrye-common-function:2.12.0`
- `io.suzaku:boopickle_2.13:1.5.0`
- `io.undertow:undertow-core:2.3.23.Final`
- `io.undertow:undertow-servlet:2.3.23.Final`
- `javax.inject:javax.inject:1`
- `javax.validation:validation-api:1.1.0.Final`
- `joda-time:joda-time:2.1`
- `net.bytebuddy:byte-buddy-agent:1.15.11`
- `net.bytebuddy:byte-buddy:1.15.11`
- `net.debasishg:redisclient_2.13:3.42`
- `net.jodah:typetools:0.6.3`
- `net.minidev:accessors-smart:2.6.0`
- `net.minidev:json-smart:2.6.0`
- `net.objecthunter:exp4j:0.4.8`
- `oauth.signpost:signpost-commonshttp4:1.2`
- `oauth.signpost:signpost-core:1.2.1.1`
- `org.apache.commons:commons-collections4:4.4`
- `org.apache.commons:commons-compress:1.27.1`
- `org.apache.commons:commons-configuration2:2.9.0`
- `org.apache.commons:commons-csv:1.14.1`
- `org.apache.commons:commons-lang3:3.18.0`
- `org.apache.commons:commons-math3:3.6.1`
- `org.apache.commons:commons-pool2:2.12.1`
- `org.apache.commons:commons-text:1.14.0`
- `org.apache.httpcomponents:httpclient:4.5.14`
- `org.apache.httpcomponents:httpcore:4.4.16`
- `org.apache.logging.log4j:log4j-api:2.24.3`
- `org.apache.maven.plugin-testing:maven-plugin-testing-harness:4.0.0-beta-3`
- `org.apache.maven.plugin-tools:maven-plugin-annotations:3.15.1`
- `org.apache.maven.resolver:maven-resolver-api:1.9.22`
- `org.apache.maven.resolver:maven-resolver-impl:1.9.22`
- `org.apache.maven.resolver:maven-resolver-named-locks:1.9.22`
- `org.apache.maven.resolver:maven-resolver-spi:1.9.22`
- `org.apache.maven.resolver:maven-resolver-util:1.9.22`
- `org.apache.maven.shared:maven-shared-utils:3.4.2`
- `org.apache.maven.wagon:wagon-provider-api:3.5.3`
- `org.apache.maven:maven-api-annotations:4.0.0-rc-2`
- `org.apache.maven:maven-api-xml:4.0.0-rc-2`
- `org.apache.maven:maven-artifact:3.9.9`
- `org.apache.maven:maven-builder-support:3.9.9`
- `org.apache.maven:maven-compat:3.9.9`
- `org.apache.maven:maven-core:3.9.9`
- `org.apache.maven:maven-model-builder:3.9.9`
- `org.apache.maven:maven-model:3.9.9`
- `org.apache.maven:maven-plugin-api:3.9.9`
- `org.apache.maven:maven-repository-metadata:3.9.9`
- `org.apache.maven:maven-resolver-provider:3.9.9`
- `org.apache.maven:maven-settings-builder:3.9.9`
- `org.apache.maven:maven-settings:3.9.9`
- `org.apache.maven:maven-xml:4.0.0-rc-2`
- `org.apache.pdfbox:fontbox:3.0.5`
- `org.apache.pdfbox:pdfbox-io:3.0.5`
- `org.apache.pdfbox:pdfbox:3.0.5`
- `org.apache.poi:poi-ooxml-lite:5.4.1`
- `org.apache.poi:poi-ooxml:5.4.1`
- `org.apache.poi:poi:5.4.1`
- `org.apache.tinkerpop:gremlin-core:3.7.4`
- `org.apache.tinkerpop:gremlin-driver:3.7.4`
- `org.apache.tinkerpop:gremlin-language:3.7.4`
- `org.apache.tinkerpop:gremlin-shaded:3.7.4`
- `org.apache.tinkerpop:gremlin-util:3.7.4`
- `org.apache.tinkerpop:tinkergraph-gremlin:3.7.4`
- `org.apache.ws.xmlschema:xmlschema-core:2.2.1`
- `org.apache.xmlbeans:xmlbeans:5.3.0`
- `org.apiguardian:apiguardian-api:1.1.2`
- `org.bitbucket.b_c:jose4j:0.9.6`
- `org.codehaus.plexus:plexus-cipher:2.0`
- `org.codehaus.plexus:plexus-classworlds:2.6.0`
- `org.codehaus.plexus:plexus-component-annotations:2.1.0`
- `org.codehaus.plexus:plexus-interpolation:1.26`
- `org.codehaus.plexus:plexus-sec-dispatcher:2.0`
- `org.codehaus.plexus:plexus-utils:3.5.1`
- `org.eclipse.microprofile.openapi:microprofile-openapi-api:4.0.2`
- `org.htmlunit:neko-htmlunit:4.6.0`
- `org.javatuples:javatuples:1.2`
- `org.jboss.logging:jboss-logging:3.6.1.Final`
- `org.jboss.threads:jboss-threads:3.8.0.Final`
- `org.jboss.xnio:xnio-api:3.8.16.Final`
- `org.jboss.xnio:xnio-nio:3.8.16.Final`
- `org.jetbrains.kotlin:kotlin-stdlib:2.0.21`
- `org.jetbrains:annotations:26.0.2`
- `org.jspecify:jspecify:1.0.0`
- `org.jvnet.jaxb2_commons:jaxb2-commons-lang:2.4`
- `org.keycloak:keycloak-common:26.3.4`
- `org.keycloak:keycloak-core:26.3.4`
- `org.mongodb:bson-record-codec:5.6.0`
- `org.mongodb:bson:5.6.0`
- `org.mongodb:mongodb-driver-core:5.6.0`
- `org.mongodb:mongodb-driver-sync:5.6.0`
- `org.objenesis:objenesis:3.3`
- `org.opentest4j:opentest4j:1.3.0`
- `org.raml:raml-parser-2:1.0.47`
- `org.raml:yagi:1.0.47`
- `org.scala-lang.modules:scala-collection-compat_2.13:2.12.0`
- `org.scala-lang.modules:scala-parser-combinators_2.13:2.4.0`
- `org.scala-lang.modules:scala-swing_2.13:3.0.0`
- `org.scala-lang:scala-library:2.13.16`
- `org.scala-lang:scala-reflect:2.13.16`
- `org.shredzone.acme4j:acme4j-client:3.5.1`
- `org.unbescape:unbescape:1.1.6.RELEASE`
- `org.wildfly.client:wildfly-client-config:1.0.1.Final`
- `org.wildfly.common:wildfly-common:1.5.4.Final-format-001`
- `org.xmlresolver:xmlresolver:6.0.19`
- `org.yaml:snakeyaml:2.0`
- `xml-apis:xml-apis:1.4.01`

</details>

<details><summary><strong>BSD (2/3-Clause / style)</strong> — ✅ Permissive (16)</summary>

- `asm:asm-commons:3.3.1`
- `asm:asm-tree:3.3.1`
- `asm:asm:3.3.1`
- `com.github.mwiede:jsch:2.27.3`
- `com.github.virtuald:curvesapi:1.08`
- `io.burt:jmespath-core:0.6.0`
- `io.burt:jmespath-jackson:0.6.0`
- `io.pebbletemplates:pebble:3.2.4`
- `org.antlr:antlr4-runtime:4.13.2`
- `org.codehaus.woodstox:stax2-api:4.2.2`
- `org.commonmark:commonmark:0.26.0`
- `org.hamcrest:hamcrest:3.0`
- `org.hsqldb:hsqldb:2.7.0`
- `org.jodd:jodd-lagarto:6.0.6`
- `org.jvnet.jaxb2_commons:jaxb2-basics-runtime:1.11.1`
- `org.ow2.asm:asm:9.7.1`

</details>

<details><summary><strong>MIT</strong> — ✅ Permissive (14)</summary>

- `com.auth0:java-jwt:4.5.0`
- `com.eatthepath:fast-uuid:0.2.0`
- `com.github.scopt:scopt_2.13:3.7.1`
- `net.sf.jopt-simple:jopt-simple:5.0.3`
- `net.sourceforge.plantuml:plantuml-mit:1.2026.6`
- `org.jsoup:jsoup:1.21.2`
- `org.mockito:mockito-core:5.16.1`
- `org.simpleflatmapper:lightning-csv:9.0.2`
- `org.simpleflatmapper:sfm-util:9.0.2`
- `org.slf4j:jcl-over-slf4j:1.7.25`
- `org.slf4j:slf4j-api:2.0.17`
- `org.slf4j:slf4j-simple:2.0.17`
- `redis.clients.authentication:redis-authx-core:0.1.1-beta2`
- `redis.clients:jedis:6.2.0`

</details>

<details><summary><strong>EPL (Eclipse, copyleft faible)</strong> — ✅ Copyleft faible (13)</summary>

- `com.sun.mail:jakarta.mail:2.0.2`
- `jakarta.annotation:jakarta.annotation-api:3.0.0`
- `jakarta.jms:jakarta.jms-api:3.1.0`
- `jakarta.servlet:jakarta.servlet-api:6.0.0`
- `junit:junit:4.13.2`
- `org.eclipse.sisu:org.eclipse.sisu.inject:0.9.0.M3`
- `org.eclipse.sisu:org.eclipse.sisu.plexus:0.9.0.M3`
- `org.junit.jupiter:junit-jupiter-api:5.12.1`
- `org.junit.jupiter:junit-jupiter-engine:5.12.1`
- `org.junit.jupiter:junit-jupiter-params:5.12.1`
- `org.junit.jupiter:junit-jupiter:5.12.1`
- `org.junit.platform:junit-platform-commons:1.12.1`
- `org.junit.platform:junit-platform-engine:1.12.1`

</details>

<details><summary><strong>LGPL (copyleft)</strong> — ✅ Copyleft (8)</summary>

- `com.github.librepdf:openpdf:3.0.0`
- `com.github.spotbugs:spotbugs-annotations:4.9.0`
- `com.google.code.findbugs:annotations:3.0.0`
- `net.sf.cssbox:cssbox:5.0.2`
- `net.sf.cssbox:jstyleparser:4.0.1`
- `org.mariadb.jdbc:mariadb-java-client:2.7.12`
- `org.xhtmlrenderer:flying-saucer-core:9.4.0`
- `org.xhtmlrenderer:flying-saucer-pdf:9.4.0`

</details>

<details><summary><strong>Apache-2.0 OU LGPL (double licence)</strong> — ✅ Copyleft (choix Apache) (6)</summary>

- `com.github.fge:btf:1.2`
- `com.github.fge:msg-simple:1.1`
- `com.github.fge:uri-template:0.9`
- `com.github.java-json-tools:jackson-coreutils:1.9`
- `com.github.java-json-tools:json-schema-core:1.2.10`
- `com.github.java-json-tools:json-schema-validator:2.2.10`

</details>

<details><summary><strong>EPL / LGPL (double licence)</strong> — ✅ Copyleft faible (5)</summary>

- `ch.qos.logback.contrib:logback-jackson:0.1.5`
- `ch.qos.logback.contrib:logback-json-classic:0.1.5`
- `ch.qos.logback.contrib:logback-json-core:0.1.5`
- `ch.qos.logback:logback-classic:1.5.18`
- `ch.qos.logback:logback-core:1.5.18`

</details>

<details><summary><strong>Bouncy Castle (MIT-style)</strong> — ✅ Permissive (4)</summary>

- `io.gatling:gatling-recorder-bc-shaded:1.81.0`
- `org.bouncycastle:bcpkix-jdk18on:1.81`
- `org.bouncycastle:bcprov-jdk18on:1.82`
- `org.bouncycastle:bcutil-jdk18on:1.81`

</details>

<details><summary><strong>CDDL / GPL (double licence)</strong> — ✅ Copyleft faible (choix CDDL) (4)</summary>

- `com.sun.mail:javax.mail:1.6.1`
- `javax.json:javax.json-api:1.0`
- `javax.xml.bind:jaxb-api:2.2.12`
- `org.glassfish:javax.json:1.0.4`

</details>

<details><summary><strong>MPL (Mozilla, copyleft faible)</strong> — ✅ Copyleft faible (3)</summary>

- `com.googlecode.juniversalchardet:juniversalchardet:1.0.3`
- `net.sf.saxon:Saxon-HE:12.9`
- `org.mozilla:rhino:1.7.7.1`

</details>

<details><summary><strong>EDL 1.0 (BSD-style)</strong> — ✅ Permissive (2)</summary>

- `com.sun.activation:jakarta.activation:2.0.1`
- `jakarta.activation:jakarta.activation-api:2.1.3`

</details>

<details><summary><strong>CDDL</strong> — ✅ Copyleft faible (1)</summary>

- `javax.activation:activation:1.1`

</details>

<details><summary><strong>Domaine public</strong> — ✅ Domaine public (1)</summary>

- `aopalliance:aopalliance:1.0`

</details>

<details><summary><strong>Gatling Highcharts (PROPRIÉTAIRE)</strong> — ❌ Propriétaire (1)</summary>

- `io.gatling.highcharts:gatling-charts-highcharts:3.14.4`

</details>

<details><summary><strong>Java HTML Tidy (zlib/MIT-style)</strong> — ✅ Permissive (1)</summary>

- `net.sf.jtidy:jtidy:r938`

</details>

<details><summary><strong>The JSON License (non-OSI)</strong> — ❌ Non-OSI (1)</summary>

- `org.json:json:20160810`

</details>

<details><summary><strong>Unicode (permissive)</strong> — ✅ Permissive (1)</summary>

- `com.ibm.icu:icu4j:77.1`

</details>

---

## Analyse d'impact — `org.json` (The JSON License)

> Analyse menée via GitHub (orgs `flexiooss` + `Flexio-corp`) pour déterminer si la seule
> dépendance **non open source / non-OSI** réellement embarquable est utilisée par le code Flexio.

### Origine

`org.json:json:20160810` n'est **jamais déclarée directement** dans un POM Flexio. Elle est
tirée **transitivement** par le SDK QuickBooks, lui-même déclaré dans ce BOM :

```
com.intuit.quickbooks-online:oauth2-platform-api:5.0.3   (SDK Intuit QuickBooks)
  └─ org.json:json:20160810   (scope compile)
```

### Usage réel dans le code Flexio

| Contexte | Usage de `org.json` | Impact licence |
|---|---|---|
| `flexio-quickbooks` (`-connector` + `-service`) et `flexio-oauth-manager` | Indirect : tirent le SDK QuickBooks → `org.json` sur le classpath, utilisé **par le SDK Intuit**, pas par le code Flexio | ⚠️ Théorique — **mais voir ci-dessous** |
| `flexio-mobile-v1-service` → `GeolocToData.java` | `import org.json.JSONObject;` présent, **mais import mort** : `JSONObject` n'est référencé nulle part dans la classe | ✅ Aucun (import inutilisé) |
| `flexapp-android` (~15 fichiers : `MyFile`, `MyImage`, `ConfigParserService`…) | Usage massif, mais projet **Gradle/Android** | ✅ Aucun — Android fournit sa **propre réimplémentation `org.json`** (réécriture Google sous **Apache 2.0**) ; l'artefact Crockford n'est pas embarqué |

### Statut QuickBooks

⚠️ **Le connecteur QuickBooks a été abandonné et n'est plus déployé en production.** La seule
chaîne qui embarquait réellement `org.json` (via le SDK Intuit) ne tourne donc plus en prod.

### Verdict

L'exposition pratique est **quasi nulle** :

- la voie QuickBooks (qui embarquait le jar) est **désactivée / non déployée** ;
- l'unique référence dans du code backend (`GeolocToData`) est un **import mort**, sans aucun
  appel à `org.json` ;
- le gros volume d'usage (app Android) repose sur l'`org.json` **Apache 2.0** de la plateforme,
  pas sur l'artefact à licence problématique.

Nuance complémentaire : Flexio étant exploité en **SaaS** (hébergé, non distribué aux clients),
la clause sensible de la *JSON License* (« *Good, not Evil* »), qui se déclenche surtout à la
**distribution de binaires**, a de toute façon une portée juridique très limitée. La gêne
résiduelle relève surtout de la **compatibilité OSI/Apache** et de la politique interne.

### Remédiation recommandée

1. **`GeolocToData.java`** — supprimer l'`import org.json.JSONObject;` mort (et les autres imports
   inutilisés). Coût nul, supprime la dernière référence de code Flexio à la librairie.
2. **QuickBooks** — déjà abandonné/non déployé ; si le module est un jour réactivé, `org.json` est
   requis en interne par le SDK Intuit (non retirable sans le casser) → à réévaluer à ce moment-là.

---

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
