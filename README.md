BuildScripts
============

Gradle scripts used for building various Java projects I've released on GitHub


## Using

Projects using `build_java_lib.gradle` must define the following properties in their `gradle.properties`:

1. javaSourceCompatibility
2. javaTargetCompatibility
3. group
4. version
5. builtBy

Local Maven publishing is supported via `gradle publishtomavenlocal`.
