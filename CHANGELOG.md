# May 26, 2018

Removed findbugs from `build_java_lib.gradle`, as it's incompatible with Java 10 and [the project is dead](https://mailman.cs.umd.edu/pipermail/findbugs-discuss/2016-November/004321.html).

I'll have to replace findbugs with something else, but this is on hold for the moment.  Gradle is planning on breaking things in their upcoming 5.0 release, so I'm delaying work on my script until I have time to rewrite it in "the Gradle 5.0 way".