# ic-spring-cloud-config
Basic Spring Cloud Config example for ItalianCoders article

# Build and run the server
    cd config-server
    mvn install
    java -jar target/config-server.jar

## Check server
    curl localhost:8060/myapp/dev

# Build and run the client
    cd config-client
    mvn install
    java -jar -Dspring.profiles.active=dev target/config-client.jar

or (for prod env)

    java -jar -Dspring.profiles.active=prod target/config-client.jar
