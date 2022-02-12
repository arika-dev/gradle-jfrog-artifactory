## Setup local artifactory
```shell
docker run --name artifactory2 -d -p 8081:8081 -p 8082:8082 docker.bintray.io/jfrog/artifactory-cpp-ce:latest
```

http://localhost:8082/ui/repos/tree/General/artifactory-build-info


## Publish to artifactory
`./gradlew build`

`./gradlew artifactoryPublish`