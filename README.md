# FunWithMaven
Maven learnings

This is very preliminary.

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

