# FunWithMaven
Maven learnings

This is very preliminary.

JAVA_HOME
(M2_HOME)
(M2) I did not need these
~/.m2
local repository
central repository
parent pom
mvn help:effective-pom
conf or settings files in m2 install and ~/.mw.
Seems out of date.
      <dependencies>
        <dependency>
          <groupId>junit</groupId>
          <artifactId>junit</artifactId>
          <version>4.8.1</version>
          <scope>test</scope>
        </dependency>
      </dependencies>

build profiles
plugin development


# Tutorial Notes
## pom
<project xmlns="http://maven.apache.org/POM/4.0.0"
         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
         xsi:schemaLocation="http://maven.apache.org/POM/4.0.0
                      http://maven.apache.org/xsd/maven-4.0.0.xsd">
    <modelVersion>4.0.0</modelVersion>
    <groupId>domain,maybe</groupId>
    <artifactId>unique artifat name</artifactId>
    <version>1.0.0</version>
</project>

## Commands
lifecycles {phases {goals} }
install = phase
Main lifecycles: clean <default> site
validate
compile
test
package
install
deploy

## Java properties
default language level is 1.5
<properties>
    <maven.compiler.target>1.8</maven.compiler.target>
    <maven.compiler.source>1.8</maven.compiler.source>
</properties>

java tvf name-of-jar
Can't actually see language level from bytecode

## IDEs
mvn eclipse:eclipse
mvn idea:idea

## Unit tests
mvn surefire-report:report
mvn surefire-report:report-only
your-project/target/site/surefire-report.html

