Test code to compare the performance of removing whitespace between two maven plugins:

com.google.code.maven-replacer-plugin::replacer::1.5.2  vs.  com.github.dantwining.whitespace-maven-plugin::whitespace-maven-plugin::1.0.4

Usage:


Each of the plugins can be activated by the respective profiles for them:

com.github.dantwining.whitespace-maven-plugin::whitespace-maven-plugin::1.0.4 can be used like so:
git reset --hard && mvn clean install -Pwhitespace-maven-plugin

OR,

com.google.code.maven-replacer-plugin::replacer::1.5.2 can be used like so:
git reset --hard && mvn clean install -Pmaven-replacer-plugin

Current Results (02-June-2014)

| Build | whitespace-maven-plugin | maven-replacer-plugin  |
| ----- | ------------- | ------------- |
| 1  | 48.4  | 48 |
| 2  | 48.1  | 47.9|
| 3  |  48  | 49|  

(All times are in seconds and are for complete builds, i.e. including compilation, building the jar etc. )

