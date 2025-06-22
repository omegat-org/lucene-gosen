# The forked version of the Lucene-Gosen

Here is a forked version of the lucene-gosen project.
A `rel-8.11` branch is a main branch of the forked project.

Lucene 8.11 is a latest Lucene which support Java 8.
Lucene 9+ requires Java 11 or Java 17.

OmegaT project releases OmegaT 6.0.x that is compiled with Java 11 and bundled with JRE 17.
The forked project is aimed to used with LanguageTool versions that uses Lucene version 8.11.3.

## Download from Maven Central

* group id : org.omegat.lucene
* artifact id : lucene-gosen

There are three types of jar files:

* lucene-gosen-<version>.jar : Only java library, not include dictionary.
* lucene-gosen-<version>-ipadic.jar : Java library with IPA dictionary.
* lucene-gosen-<version>-naist-chasen.jar : Java library with Naist Chasen dictionary

## Installation with Apache Lucene 8.11.3:

### Using Maven

Add dependency to pom.xml.

```
    <dependencies>
        <dependency>
            <groupId>org.omegat.lucene</groupId>
            <artifactId>lucene-gosen</artifactId>
            <version>8.11.1</version>
            <classifier>ipadic</classifier>
        </dependency>
        ...
    </dependencies>
```

### Non Maven project

1. Download jar file from Maven Central Repository
2. Add this jar file to your classpath, and use GosenAnalyzer, or make your own analyzer from
   the various filters. Its recommended you extend ReusableAnalyzerBase to make any custom analyzer!

## Build

You can build the project using Gradle. And you should use `gradlew` command.

Build only jar file without dictionary

```
$ ./gradlew jar
```

Build jar file with IPA dictionary

```
$ ./gradlew jarWithIpaDic
```

Build jar file with Naist Chasen dictionary

```
$ ./gradlew jarWithNaistChasen
```
