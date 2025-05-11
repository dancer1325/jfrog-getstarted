# how to build locally?
* set JDK v11
* `mvn clean install`

# how to build the project & resolve project dependencies -- from -- Artifactory?
* | this path
  * `jf mvn-config`
    * configure the project's repositories
    * Problems: 
      * Problem1: "failed getting repositories list: failed getting virtual repositories list: invalid character '<' looking for beginning of value"
        * Solution: ⚠️trigger 1! ⚠️
  * `jf mvn clean install -f pom.xml --build-name maven-challenge --build-number 1.0.0`
    * build the project / resolve the project dependencies -- from -- Artifactory
    * Problems:
      * Problem1: "Plugin org.apache.maven.plugins:maven-clean-plugin:3.2.0 or one of its dependencies could not be resolved.  status code: 403, reason phrase: Forbidden (403)"
        * Solution: TODO:
  * `jf rt bp maven-challenge 1.0.0`
    * publish build info | Artifactory
