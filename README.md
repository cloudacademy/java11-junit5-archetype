# Maven Quickstart Archetype - Java 11 + JUnit5

## Summary
Used to provide a Maven archetype for Java 11 and JUnit5. You can use this to quickly generate new Java 11 and JUnit 5 TDD project layouts.

## Prerequisites
* JDK 11
* Maven 3

## Install Archetype Locally

To install the archetype in your local repository execute the following commands:

```bash
git clone https://github.com/cloudacademy/java11-junit5-archetype.git
cd java11-junit5-archetype
mvn clean install
```

## Maven Create/Generate New Java Project

```bash
mvn archetype:generate \
 -DarchetypeGroupId=com.cloudacademy.devops \
 -DarchetypeArtifactId=java11-junit5-archetype \
 -DarchetypeVersion=1.0.0-SNAPSHOT \
 -DgroupId=com.example \
 -DartifactId=my-project \
 -Dversion=1.0.0-SNAPSHOT \
 -DinteractiveMode=false
```

## Build and Run New Java Project

### Step 1: Build, Test, and Package Executable Jar

```bash
cd my-project
mvn clean package
```

### Step 2: Run

```bash
java -jar target/my-project-1.0.0-SNAPSHOT-jar-with-dependencies.jar
```

Should result with the following message:

```
CloudAcademy DevOps 2020!!
```

:metal:
