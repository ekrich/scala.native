Scala Native
------------
>Scala native feature apps and tests, built on Apple M1.

Install
-------
>See http://www.scala-native.org/en/latest/user/setup.html for details.
1. brew install llvm

Notes
-----
1. In crossproject mode, Sbt fails to find Scalatest dependencies; yet JVM and Native tests pass.

Questions
---------
1. How to create Apple M1 console app?

Test
----
1. sbt clean test

Run
---
1. target/scala-2.13/scala-native-out
2. file target/scala-2.13/scala-native-out ( Mach-O 64-bit executable arm64 )

Publish
-------
1. sbt clean compile package publishLocal

Cross Project
-------------
>Cross project is currently disabled. See plugins.sbt and build.sbt for details.

Resources
---------
1. Scala Native Docs - http://www.scala-native.org/en/latest/index.html
2. Scala Native Intro Video - https://www.youtube.com/watch?v=u2CnE-sRdBw
3. Scala Native Performance - https://medium.com/virtuslab/revisiting-scala-native-performance-67029089f241