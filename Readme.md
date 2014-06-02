Test code to compare the performance of removing whitespace between two maven plugins:

com.google.code.maven-replacer-plugin::replacer::1.5.2  vs.  com.github.dantwining.whitespace-maven-plugin::whitespace-maven-plugin::1.0.4

Usage:


Each of the plugins can be activated by the respective profiles for them:

com.github.dantwining.whitespace-maven-plugin::whitespace-maven-plugin::1.0.4 can be used like so:
git reset --hard && mvn clean install -Pwhitespace-maven-plugin

OR,

com.google.code.maven-replacer-plugin::replacer::1.5.2 can be used like so:
git reset --hard && mvn clean install -Pmaven-replacer-plugin


