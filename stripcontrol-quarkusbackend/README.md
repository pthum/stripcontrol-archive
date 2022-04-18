# stripcontrol-quarkusbackend project

> [Deprecated] Stripcontrol backend application made with Quarkus.

You will need the `stripcontrol-ledhandling` project and it's dependencies at [this state](https://github.com/pthum/stripcontrol/commit/6150a5e99b79718501da4379c5693f325c6e1aca) to get this running.

## Running the application in dev mode

You can run your application in dev mode that enables live coding using:
```
./mvnw quarkus:dev
```

## Packaging and running the application

The application can be packaged using `./mvnw package`.
It produces the `stripcontrol-quarkusbackend-1.0.0-SNAPSHOT-runner.jar` file in the `/target` directory.
Be aware that it’s not an _über-jar_ as the dependencies are copied into the `target/lib` directory.

The application is now runnable using `java -jar target/stripcontrol-quarkusbackend-1.0.0-SNAPSHOT-runner.jar`.

## Creating a native executable

You can create a native executable using: `./mvnw package -Pnative`.

Or, if you don't have GraalVM installed, you can run the native executable build in a container using: `./mvnw package -Pnative -Dquarkus.native.container-build=true`.

You can then execute your native executable with: `./target/stripcontrol-quarkusbackend-1.0.0-SNAPSHOT-runner`

If you want to learn more about building native executables, please consult https://quarkus.io/guides/building-native-image.