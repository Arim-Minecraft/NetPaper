NetPaper
===========

Fork of Paper 1.8.8 designed for Java 11 which includes a built-in slf4j binding. Unlike other forks, NetPaper is oriented toward developers. Say goodbye to JUL logging. Embrace Java 11 features.

Information
------

The slf4j binding is based on version *1.7.25* of slf4j. To ensure compatibility, one should build against this version. The slf4j is implemented in whole with the exception of markers - the binding is marker agnostic. However, MDC *is* supported.

The underlying netty version for NetPaper has been changed in 2 ways. First, it has been updated to 4.0.34, from 4.0.23. Note that 4.0.34 alone is not sufficient for JDK 11 support. Second, specific changes from newer netty versions have been backported to a fork of 4.0.34, which may be viewed here: https://github.com/Arim-Minecraft/netty.

How To
------

NetPaper is designed for **JDK 11** or above. Do not complain if you use it on Java 8 and experience errors.

You need to compile NetPaper from source. To do this, you need java, git, maven, and an internet connection.

Clone this repo using `git clone https://github.com/Arim-Minecraft/NetPaper.git`. Navigate to the directory and run ./build.sh from *bash*. The server JAR will be in PaperSpigot-Server/target/NetPaper.jar.

Special Thanks To:
-------------

* The netty developers. Minecraft relies on netty's fast performance.
* PaperMC of course! For making PaperSpigot to begin with.
