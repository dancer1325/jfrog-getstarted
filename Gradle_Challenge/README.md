# how to build locally?
* TODO:           
            
# how to build the project & resolve project dependencies -- from -- Artifactory?
* | this path
  * `jf gradle-config`
    * configure the project's repositories
  * `jf gradle clean artifactoryPublish -b path/to/build.gradle  --build-name gradle-challenge --build-number 1.0.0`
    * build the project / resolve the project dependencies -- from -- Artifactory
  * `jf rt bp gradle-challenge 1.0.0`
    * publish build info | Artifactory

