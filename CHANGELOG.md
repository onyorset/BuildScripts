# May 8, 2021

Completely rewritten.  The new version is a simplified implementation of existing behavior.  It also adds support for local Maven publishing.

Gradle version compatibility is an ever-changing target, but what I can say is that this release is known to work with Gradle 7.0.

Projects using `build_java_lib.gradle` must define the following properties in their `gradle.properties`:

1. javaSourceCompatibility
2. javaTargetCompatibility
3. group
4. version
5. builtBy


# May 26, 2018

Removed findbugs from `build_java_lib.gradle`, as it's incompatible with Java 10 and [the project is dead](https://mailman.cs.umd.edu/pipermail/findbugs-discuss/2016-November/004321.html).

I'll have to replace findbugs with something else, but this is on hold for the moment.  Gradle is planning on breaking things in their upcoming 5.0 release, so I'm delaying work on my script until I have time to rewrite it in "the Gradle 5.0 way".