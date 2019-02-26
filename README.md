# generate lagom maven project
One more Lagom java maven getting started project...

# EASY AS 1-2-3

```bash
mvn archetype:generate  -DarchetypeGroupId=com.lightbend.lagom \
                        -DarchetypeArtifactId=maven-archetype-lagom-java \
                        -DarchetypeVersion=1.4.11 \
                        -DgroupId=com.github.daggerok \
                        -DartifactId=lagom-mvn \
                        -Dversion=1.0.0-SNAPSHOT \
                        -Dpackage=com.github.daggerok \
                        -B
cd lagom-mvn/
mvn -N io.takari:maven:wrapper -Dmaven=3.6.0
./mvnw clean package
./mvnw lagom:runAll

http :9000/api/hello/Lagom
```

## resources

- [lagom framework](https://www.lagomframework.com/)
- [lagom documentation](https://www.lagomframework.com/documentation/)
- [generate lagom maven project guide](https://www.lagomframework.com/documentation/1.4.x/java/GettingStartedMaven.html#Generate-a-project-with-the-Lagom-archetype)
