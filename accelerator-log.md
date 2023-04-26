# Accelerator Log

## Options
```json
{
  "bsGitBranch" : "main",
  "bsGitRepository" : "github.com?owner=igodwin&repo=where-for-dinner",
  "cacheName" : "cache-where-for-dinner",
  "cacheType" : "redisCache",
  "dbName" : "db-where-for-dinner",
  "dbType" : "mysql",
  "enableCloudEvents" : false,
  "enableSecurity" : false,
  "numRabbitMQClusterNodes" : 1,
  "projectName" : "where-for-dinner",
  "rabbitMQName" : "rmq-where-for-dinner",
  "serviceNamespace" : "service-instances",
  "workloadNamespace" : "workloads"
}
```
## Log
```
┏ engine (Chain)
┃  Info Running Chain(GeneratorValidationTransform, UniquePath)
┃ ┏ ┏ engine.transformations[0].validated (Combo)
┃ ┃ ┃  Info Combo running as Chain
┃ ┃ ┃ engine.transformations[0].validated.delegate (Chain)
┃ ┃ ┃  Info Running Chain(Merge, UniquePath)
┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0] (Merge)
┃ ┃ ┃ ┃  Info Running Merge(Combo, Combo, Combo, Combo, Combo, Combo, Combo, Combo, Combo)
┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].sources[0] (Combo)
┃ ┃ ┃ ┃ ┃  Info Combo running as Exclude
┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.delegate.transformations[0].sources[0].delegate (Exclude)
┃ ┃ ┃ ┃ ┃  Info Will exclude [**/templates/**, **/icons/**, **/.git/**, **/deployment/**]
┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug catalog/components/where-for-dinner-api-gateway/where-for-dinner-api-gateway.yaml didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug catalog/components/where-for-dinner-availability/where-for-dinner-availability.yaml didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug catalog/components/where-for-dinner-notify/where-for-dinner-notify.yaml didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug catalog/components/where-for-dinner-search/where-for-dinner-search.yaml didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug catalog/components/where-for-dinner-search-proc/where-for-dinner-search-proc.yaml didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug catalog/components/where-for-dinner-ui/where-for-dinner-ui.yaml didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug catalog/groups/org.yaml didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug catalog/resources/db/where-for-dinner-db-resource.yaml didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug catalog/resources/messaging/where-for-dinner-messaging-resource.yaml didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug catalog/systems/where-for-dinner-system.yaml didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug doc/TAPDeployment.md didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug doc/images/AppHomeScreen.png didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug doc/images/DinnerHighLevelArch.png didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug doc/images/KnativeEventing.png didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug doc/images/SCSMessaging.png didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug icons/where-for-dinner.png matched [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> excluded
┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug templates/appSSOInstance.yaml matched [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> excluded
┃ ┃ ┃ ┃ ┃ Debug templates/clientRegistrationResourceClaim.yaml matched [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> excluded
┃ ┃ ┃ ┃ ┃ Debug templates/knEventing.yaml matched [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> excluded
┃ ┃ ┃ ┃ ┃ Debug templates/mysqlInstance.yaml matched [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> excluded
┃ ┃ ┃ ┃ ┃ Debug templates/mysqlResourceClaim.yaml matched [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> excluded
┃ ┃ ┃ ┃ ┃ Debug templates/redisInstance.yaml matched [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> excluded
┃ ┃ ┃ ┃ ┃ Debug templates/redisResourceClaim.yaml matched [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> excluded
┃ ┃ ┃ ┃ ┃ Debug templates/rmqCluster.yaml matched [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> excluded
┃ ┃ ┃ ┃ ┃ Debug templates/rmqResourceClaim.yaml matched [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> excluded
┃ ┃ ┃ ┃ ┃ Debug templates/workloads.yaml matched [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> excluded
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-api-gateway/.gitignore didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-api-gateway/Tiltfile didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-api-gateway/config/workload.yaml didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-api-gateway/pom.xml didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-api-gateway/src/main/java/com/java/example/tanzu/wherefordinner/DinnerAPIGatewayApplication.java didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-api-gateway/src/main/resources/application.yaml didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/.gitignore didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/.mvn/wrapper/maven-wrapper.properties didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/Tiltfile didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/config/workload.yaml didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/mvnw didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/mvnw.cmd didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/pom.xml didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/main/java/com/java/example/tanzu/wherefordinner/WhereForDinnerAvailabilityApplication.java didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/main/java/com/java/example/tanzu/wherefordinner/config/OAuth2BindingsPropertiesProcessor.java didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/main/java/com/java/example/tanzu/wherefordinner/config/WebSecurityConfig.java didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/main/java/com/java/example/tanzu/wherefordinner/entity/Availability.java didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/main/java/com/java/example/tanzu/wherefordinner/entity/AvailabilityWindow.java didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/main/java/com/java/example/tanzu/wherefordinner/function/AvailabilitySink.java didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/main/java/com/java/example/tanzu/wherefordinner/model/Availability.java didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/main/java/com/java/example/tanzu/wherefordinner/repository/AvailabilityRepository.java didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/main/java/com/java/example/tanzu/wherefordinner/repository/AvailabilityWindowRepository.java didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/main/java/com/java/example/tanzu/wherefordinner/resources/AvailabilityResource.java didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/main/resources/META-INF/spring.factories didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/main/resources/application.yaml didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/main/resources/schema-h2.sql didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/main/resources/schema-mysql.sql didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/main/resources/schema-postgresql.sql didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/test/java/com/java/example/tanzu/wherefordinner/WhereForDinnerAvailabilityApplicationTests.java didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-crawler/.gitignore didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-crawler/.mvn/wrapper/maven-wrapper.properties didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-crawler/config/workload.yaml didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-crawler/mvnw didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-crawler/mvnw.cmd didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-crawler/pom.xml didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-crawler/src/main/java/com/java/example/tanzu/wherefordinner/WhereForDinnerCrawlerApplication.java didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-crawler/src/main/java/com/java/example/tanzu/wherefordinner/config/StaticDiningAvailability.java didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-crawler/src/main/java/com/java/example/tanzu/wherefordinner/model/Availability.java didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-crawler/src/main/java/com/java/example/tanzu/wherefordinner/model/SearchCriteria.java didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-crawler/src/main/java/com/java/example/tanzu/wherefordinner/resources/LocalRandomSearcher.java didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-crawler/src/main/java/com/java/example/tanzu/wherefordinner/resources/SearchResource.java didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-crawler/src/main/resources/application.properties didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-crawler/src/main/resources/application.yml didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-crawler/src/test/java/com/java/example/tanzu/wherefordinner/WhereForDinnerCrawlerApplicationTests.java didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/.gitignore didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/.mvn/wrapper/maven-wrapper.properties didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/README.md didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/Tiltfile didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/config/workload.yaml didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/mvnw didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/mvnw.cmd didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/pom.xml didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/src/main/java/com/java/example/tanzu/wherefordinner/WhereForDinnerNotifyApplication.java didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/src/main/java/com/java/example/tanzu/wherefordinner/config/EmailMessageConfigProperties.java didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/src/main/java/com/java/example/tanzu/wherefordinner/config/PublisherConfiguration.java didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/src/main/java/com/java/example/tanzu/wherefordinner/functions/AvailabilitySink.java didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/src/main/java/com/java/example/tanzu/wherefordinner/model/Availability.java didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/src/main/java/com/java/example/tanzu/wherefordinner/publisher/EmailPublisher.java didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/src/main/java/com/java/example/tanzu/wherefordinner/publisher/LoggerPublisher.java didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/src/main/java/com/java/example/tanzu/wherefordinner/publisher/Publisher.java didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/src/main/resources/application.yml didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/src/test/java/com/java/example/tanzu/wherefordinner/WhereForDinnerNotifyApplicationTests.java didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/.gitignore didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/.mvn/wrapper/maven-wrapper.properties didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/README.md didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/Tiltfile didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/catalog-info.yaml didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/config/workload.yaml didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/mvnw didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/mvnw.cmd didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/pom.xml didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/main/java/com/java/example/tanzu/wherefordinner/WhereForDinnerResApplication.java didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/main/java/com/java/example/tanzu/wherefordinner/config/OAuth2BindingsPropertiesProcessor.java didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/main/java/com/java/example/tanzu/wherefordinner/config/WebSecurityConfig.java didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/main/java/com/java/example/tanzu/wherefordinner/entity/Search.java didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/main/java/com/java/example/tanzu/wherefordinner/functions/SearchSupplier.java didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/main/java/com/java/example/tanzu/wherefordinner/repository/SearchRepository.java didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/main/java/com/java/example/tanzu/wherefordinner/resources/SearchResource.java didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/main/resources/META-INF/spring.factories didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/main/resources/application.yml didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/main/resources/schema-h2.sql didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/main/resources/schema-mysql.sql didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/main/resources/schema-postgresql.sql didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/test/java/com/java/example/tanzu/wherefordinner/SpringBaseTest.java didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/test/java/com/java/example/tanzu/wherefordinner/WhereForDinnerResApplicationTests.java didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/test/java/com/java/example/tanzu/wherefordinner/repository/SearchRepositoryTest.java didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/test/resources/application.yml didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/.gitignore didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/.mvn/wrapper/maven-wrapper.properties didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/README.md didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/Tiltfile didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/config/workload.yaml didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/mvnw didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/mvnw.cmd didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/pom.xml didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/src/main/java/com/java/example/tanzu/wherefordinner/WhereForDinnerSearchProcApplication.java didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/src/main/java/com/java/example/tanzu/wherefordinner/config/StaticDiningAvailability.java didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/src/main/java/com/java/example/tanzu/wherefordinner/feign/CrawlerClient.java didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/src/main/java/com/java/example/tanzu/wherefordinner/functions/Search.java didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/src/main/java/com/java/example/tanzu/wherefordinner/model/Availability.java didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/src/main/java/com/java/example/tanzu/wherefordinner/model/SearchCriteria.java didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/src/main/java/com/java/example/tanzu/wherefordinner/processor/SearchProcessor.java didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/src/main/java/com/java/example/tanzu/wherefordinner/processor/cache/HashCache.java didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/src/main/java/com/java/example/tanzu/wherefordinner/processor/cache/MemoryHashCache.java didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/src/main/java/com/java/example/tanzu/wherefordinner/processor/cache/RedisHashCache.java didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/src/main/java/com/java/example/tanzu/wherefordinner/searcher/Searcher.java didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/src/main/java/com/java/example/tanzu/wherefordinner/searcher/impl/CrawlerSearcher.java didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/src/main/java/com/java/example/tanzu/wherefordinner/searcher/impl/LocalRandomSearcher.java didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/src/main/resources/application.yml didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/src/test/java/com/java/example/tanzu/wherefordinner/WhereForDinnerSearchProcApplicationTests.java didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/.gitignore didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/README.md didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/httpproxy.yaml didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/package-lock.json didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/package.json didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/public/favicon.png didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/public/index.html didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/public/manifest.json didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/public/robots.txt didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/src/App.css didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/src/App.js didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/src/App.test.js didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/src/Availability.js didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/src/DiningNames.js didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/src/DiningSearch.js didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/src/DiningSearches.js didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/src/DiningTypes.js didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/src/SearchDefForm.js didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/src/TimeWindow.js didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/src/images/delete.png didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/src/index.css didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/src/index.js didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/src/logo.svg didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/src/reportWebVitals.js didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┗ Debug where-for-dinner-ui/src/setupTests.js didn't match [**/templates/**, **/icons/**, **/.git/**, **/deployment/**] -> included
┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].sources[1] (Combo)
┃ ┃ ┃ ┃ ┃  Info Combo running as Chain
┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.delegate.transformations[0].sources[1].delegate (Chain)
┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, YTT, RewritePath, InvokeFragment)
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].sources[1].delegate.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃  Info Will include [**/templates/workloads.yaml]
┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/components/where-for-dinner-api-gateway/where-for-dinner-api-gateway.yaml didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/components/where-for-dinner-availability/where-for-dinner-availability.yaml didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/components/where-for-dinner-notify/where-for-dinner-notify.yaml didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/components/where-for-dinner-search/where-for-dinner-search.yaml didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/components/where-for-dinner-search-proc/where-for-dinner-search-proc.yaml didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/components/where-for-dinner-ui/where-for-dinner-ui.yaml didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/groups/org.yaml didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/resources/db/where-for-dinner-db-resource.yaml didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/resources/messaging/where-for-dinner-messaging-resource.yaml didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/systems/where-for-dinner-system.yaml didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug doc/TAPDeployment.md didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug doc/images/AppHomeScreen.png didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug doc/images/DinnerHighLevelArch.png didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug doc/images/KnativeEventing.png didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug doc/images/SCSMessaging.png didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug icons/where-for-dinner.png didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug templates/appSSOInstance.yaml didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug templates/clientRegistrationResourceClaim.yaml didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug templates/knEventing.yaml didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug templates/mysqlInstance.yaml didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug templates/mysqlResourceClaim.yaml didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug templates/redisInstance.yaml didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug templates/redisResourceClaim.yaml didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug templates/rmqCluster.yaml didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug templates/rmqResourceClaim.yaml didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug templates/workloads.yaml matched [**/templates/workloads.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-api-gateway/.gitignore didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-api-gateway/Tiltfile didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-api-gateway/config/workload.yaml didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-api-gateway/pom.xml didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-api-gateway/src/main/java/com/java/example/tanzu/wherefordinner/DinnerAPIGatewayApplication.java didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-api-gateway/src/main/resources/application.yaml didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/.gitignore didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/.mvn/wrapper/maven-wrapper.properties didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/Tiltfile didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/config/workload.yaml didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/mvnw didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/mvnw.cmd didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/pom.xml didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/main/java/com/java/example/tanzu/wherefordinner/WhereForDinnerAvailabilityApplication.java didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/main/java/com/java/example/tanzu/wherefordinner/config/OAuth2BindingsPropertiesProcessor.java didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/main/java/com/java/example/tanzu/wherefordinner/config/WebSecurityConfig.java didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/main/java/com/java/example/tanzu/wherefordinner/entity/Availability.java didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/main/java/com/java/example/tanzu/wherefordinner/entity/AvailabilityWindow.java didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/main/java/com/java/example/tanzu/wherefordinner/function/AvailabilitySink.java didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/main/java/com/java/example/tanzu/wherefordinner/model/Availability.java didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/main/java/com/java/example/tanzu/wherefordinner/repository/AvailabilityRepository.java didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/main/java/com/java/example/tanzu/wherefordinner/repository/AvailabilityWindowRepository.java didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/main/java/com/java/example/tanzu/wherefordinner/resources/AvailabilityResource.java didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/main/resources/META-INF/spring.factories didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/main/resources/application.yaml didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/main/resources/schema-h2.sql didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/main/resources/schema-mysql.sql didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/main/resources/schema-postgresql.sql didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/test/java/com/java/example/tanzu/wherefordinner/WhereForDinnerAvailabilityApplicationTests.java didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-crawler/.gitignore didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-crawler/.mvn/wrapper/maven-wrapper.properties didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-crawler/config/workload.yaml didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-crawler/mvnw didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-crawler/mvnw.cmd didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-crawler/pom.xml didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-crawler/src/main/java/com/java/example/tanzu/wherefordinner/WhereForDinnerCrawlerApplication.java didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-crawler/src/main/java/com/java/example/tanzu/wherefordinner/config/StaticDiningAvailability.java didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-crawler/src/main/java/com/java/example/tanzu/wherefordinner/model/Availability.java didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-crawler/src/main/java/com/java/example/tanzu/wherefordinner/model/SearchCriteria.java didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-crawler/src/main/java/com/java/example/tanzu/wherefordinner/resources/LocalRandomSearcher.java didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-crawler/src/main/java/com/java/example/tanzu/wherefordinner/resources/SearchResource.java didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-crawler/src/main/resources/application.properties didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-crawler/src/main/resources/application.yml didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-crawler/src/test/java/com/java/example/tanzu/wherefordinner/WhereForDinnerCrawlerApplicationTests.java didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/.gitignore didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/.mvn/wrapper/maven-wrapper.properties didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/README.md didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/Tiltfile didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/config/workload.yaml didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/mvnw didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/mvnw.cmd didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/pom.xml didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/src/main/java/com/java/example/tanzu/wherefordinner/WhereForDinnerNotifyApplication.java didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/src/main/java/com/java/example/tanzu/wherefordinner/config/EmailMessageConfigProperties.java didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/src/main/java/com/java/example/tanzu/wherefordinner/config/PublisherConfiguration.java didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/src/main/java/com/java/example/tanzu/wherefordinner/functions/AvailabilitySink.java didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/src/main/java/com/java/example/tanzu/wherefordinner/model/Availability.java didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/src/main/java/com/java/example/tanzu/wherefordinner/publisher/EmailPublisher.java didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/src/main/java/com/java/example/tanzu/wherefordinner/publisher/LoggerPublisher.java didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/src/main/java/com/java/example/tanzu/wherefordinner/publisher/Publisher.java didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/src/main/resources/application.yml didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/src/test/java/com/java/example/tanzu/wherefordinner/WhereForDinnerNotifyApplicationTests.java didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/.gitignore didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/.mvn/wrapper/maven-wrapper.properties didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/README.md didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/Tiltfile didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/catalog-info.yaml didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/config/workload.yaml didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/mvnw didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/mvnw.cmd didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/pom.xml didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/main/java/com/java/example/tanzu/wherefordinner/WhereForDinnerResApplication.java didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/main/java/com/java/example/tanzu/wherefordinner/config/OAuth2BindingsPropertiesProcessor.java didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/main/java/com/java/example/tanzu/wherefordinner/config/WebSecurityConfig.java didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/main/java/com/java/example/tanzu/wherefordinner/entity/Search.java didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/main/java/com/java/example/tanzu/wherefordinner/functions/SearchSupplier.java didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/main/java/com/java/example/tanzu/wherefordinner/repository/SearchRepository.java didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/main/java/com/java/example/tanzu/wherefordinner/resources/SearchResource.java didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/main/resources/META-INF/spring.factories didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/main/resources/application.yml didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/main/resources/schema-h2.sql didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/main/resources/schema-mysql.sql didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/main/resources/schema-postgresql.sql didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/test/java/com/java/example/tanzu/wherefordinner/SpringBaseTest.java didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/test/java/com/java/example/tanzu/wherefordinner/WhereForDinnerResApplicationTests.java didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/test/java/com/java/example/tanzu/wherefordinner/repository/SearchRepositoryTest.java didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/test/resources/application.yml didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/.gitignore didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/.mvn/wrapper/maven-wrapper.properties didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/README.md didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/Tiltfile didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/config/workload.yaml didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/mvnw didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/mvnw.cmd didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/pom.xml didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/src/main/java/com/java/example/tanzu/wherefordinner/WhereForDinnerSearchProcApplication.java didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/src/main/java/com/java/example/tanzu/wherefordinner/config/StaticDiningAvailability.java didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/src/main/java/com/java/example/tanzu/wherefordinner/feign/CrawlerClient.java didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/src/main/java/com/java/example/tanzu/wherefordinner/functions/Search.java didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/src/main/java/com/java/example/tanzu/wherefordinner/model/Availability.java didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/src/main/java/com/java/example/tanzu/wherefordinner/model/SearchCriteria.java didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/src/main/java/com/java/example/tanzu/wherefordinner/processor/SearchProcessor.java didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/src/main/java/com/java/example/tanzu/wherefordinner/processor/cache/HashCache.java didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/src/main/java/com/java/example/tanzu/wherefordinner/processor/cache/MemoryHashCache.java didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/src/main/java/com/java/example/tanzu/wherefordinner/processor/cache/RedisHashCache.java didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/src/main/java/com/java/example/tanzu/wherefordinner/searcher/Searcher.java didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/src/main/java/com/java/example/tanzu/wherefordinner/searcher/impl/CrawlerSearcher.java didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/src/main/java/com/java/example/tanzu/wherefordinner/searcher/impl/LocalRandomSearcher.java didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/src/main/resources/application.yml didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/src/test/java/com/java/example/tanzu/wherefordinner/WhereForDinnerSearchProcApplicationTests.java didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/.gitignore didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/README.md didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/httpproxy.yaml didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/package-lock.json didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/package.json didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/public/favicon.png didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/public/index.html didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/public/manifest.json didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/public/robots.txt didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/src/App.css didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/src/App.js didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/src/App.test.js didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/src/Availability.js didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/src/DiningNames.js didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/src/DiningSearch.js didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/src/DiningSearches.js didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/src/DiningTypes.js didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/src/SearchDefForm.js didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/src/TimeWindow.js didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/src/images/delete.png didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/src/index.css didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/src/index.js didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/src/logo.svg didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/src/reportWebVitals.js didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┗ Debug where-for-dinner-ui/src/setupTests.js didn't match [**/templates/workloads.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].sources[1].delegate.transformations[1] (YTT)
┃ ┃ ┃ ┃ ┃ ┃ Debug Wrote values file with json content:   {"bsGitBranch":"main","artifactVersion":"0.0.1-beta","bsGitRepository":"github.com?owner=igodwin&repo=where-for-dinner","dbName":"db-where-for-dinner","dbType":"mysql","rabbitMQName":"rmq-where-for-dinner","enableCloudEvents":false,"enableSecurity":false,"cacheName":"cache-where-for-dinner","numRabbitMQClusterNodes":1,"artifactId":"where-for-dinner","serviceNamespace":"service-instances","projectName":"where-for-dinner","workloadNamespace":"workloads","cacheType":"redisCache"}
┃ ┃ ┃ ┃ ┃ ┗  Info Shelling out to YTT with args: [ytt, -f, /tmp/ytt-input962210211206795768, --data-values-file, /tmp/accelerator-options14654274393670320784.json, --output-files, /tmp/ytt-output4251735358914808235]
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].sources[1].delegate.transformations[2] (RewritePath)
┃ ┃ ┃ ┃ ┃ ┗ Debug Path 'templates/workloads.yaml' matched 'templates/workloads.yaml' with groups {g0=templates/workloads.yaml} and was rewritten to 'config/developer/workloads.yaml'
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].sources[1].delegate.transformations[3] (InvokeFragment)
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].sources[1].delegate.transformations[3].validated (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Condition (#bsGitRepository != null) evaluated to true
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Let
┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.delegate.transformations[0].sources[1].delegate.transformations[3].validated.delegate (Let)
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug Adding symbol repoUrl with value 'https://github.com?owner=igodwin&repo=where-for-dinner'
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].sources[1].delegate.transformations[3].validated.delegate.in (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(OpenRewriteRecipe, ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ╺ engine.transformations[0].validated.delegate.transformations[0].sources[1].delegate.transformations[3].validated.delegate.in.transformations[0] (OpenRewriteRecipe)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].sources[1].delegate.transformations[3].validated.delegate.in.transformations[1] (ReplaceText)
┃ ┃ ┃ ┃ ┗ ┗ ┗ ┗ ┗  Info Will replace regex '(?<beforeBranch>[\s\S]+)(?<branch>branch: [\S]+)(?<rest>[\S\s]*)' with '${beforeBranch}branc...(truncated)'
┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].sources[2] (Combo)
┃ ┃ ┃ ┃ ┃  Info Combo running as Chain
┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.delegate.transformations[0].sources[2].delegate (Chain)
┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, YTT, RewritePath)
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].sources[2].delegate.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃  Info Will include [**/rmqCluster.yaml]
┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/components/where-for-dinner-api-gateway/where-for-dinner-api-gateway.yaml didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/components/where-for-dinner-availability/where-for-dinner-availability.yaml didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/components/where-for-dinner-notify/where-for-dinner-notify.yaml didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/components/where-for-dinner-search/where-for-dinner-search.yaml didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/components/where-for-dinner-search-proc/where-for-dinner-search-proc.yaml didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/components/where-for-dinner-ui/where-for-dinner-ui.yaml didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/groups/org.yaml didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/resources/db/where-for-dinner-db-resource.yaml didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/resources/messaging/where-for-dinner-messaging-resource.yaml didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/systems/where-for-dinner-system.yaml didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug doc/TAPDeployment.md didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug doc/images/AppHomeScreen.png didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug doc/images/DinnerHighLevelArch.png didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug doc/images/KnativeEventing.png didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug doc/images/SCSMessaging.png didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug icons/where-for-dinner.png didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug templates/appSSOInstance.yaml didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug templates/clientRegistrationResourceClaim.yaml didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug templates/knEventing.yaml didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug templates/mysqlInstance.yaml didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug templates/mysqlResourceClaim.yaml didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug templates/redisInstance.yaml didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug templates/redisResourceClaim.yaml didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug templates/rmqCluster.yaml matched [**/rmqCluster.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug templates/rmqResourceClaim.yaml didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug templates/workloads.yaml didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-api-gateway/.gitignore didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-api-gateway/Tiltfile didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-api-gateway/config/workload.yaml didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-api-gateway/pom.xml didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-api-gateway/src/main/java/com/java/example/tanzu/wherefordinner/DinnerAPIGatewayApplication.java didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-api-gateway/src/main/resources/application.yaml didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/.gitignore didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/.mvn/wrapper/maven-wrapper.properties didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/Tiltfile didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/config/workload.yaml didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/mvnw didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/mvnw.cmd didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/pom.xml didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/main/java/com/java/example/tanzu/wherefordinner/WhereForDinnerAvailabilityApplication.java didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/main/java/com/java/example/tanzu/wherefordinner/config/OAuth2BindingsPropertiesProcessor.java didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/main/java/com/java/example/tanzu/wherefordinner/config/WebSecurityConfig.java didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/main/java/com/java/example/tanzu/wherefordinner/entity/Availability.java didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/main/java/com/java/example/tanzu/wherefordinner/entity/AvailabilityWindow.java didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/main/java/com/java/example/tanzu/wherefordinner/function/AvailabilitySink.java didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/main/java/com/java/example/tanzu/wherefordinner/model/Availability.java didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/main/java/com/java/example/tanzu/wherefordinner/repository/AvailabilityRepository.java didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/main/java/com/java/example/tanzu/wherefordinner/repository/AvailabilityWindowRepository.java didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/main/java/com/java/example/tanzu/wherefordinner/resources/AvailabilityResource.java didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/main/resources/META-INF/spring.factories didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/main/resources/application.yaml didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/main/resources/schema-h2.sql didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/main/resources/schema-mysql.sql didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/main/resources/schema-postgresql.sql didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/test/java/com/java/example/tanzu/wherefordinner/WhereForDinnerAvailabilityApplicationTests.java didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-crawler/.gitignore didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-crawler/.mvn/wrapper/maven-wrapper.properties didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-crawler/config/workload.yaml didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-crawler/mvnw didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-crawler/mvnw.cmd didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-crawler/pom.xml didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-crawler/src/main/java/com/java/example/tanzu/wherefordinner/WhereForDinnerCrawlerApplication.java didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-crawler/src/main/java/com/java/example/tanzu/wherefordinner/config/StaticDiningAvailability.java didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-crawler/src/main/java/com/java/example/tanzu/wherefordinner/model/Availability.java didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-crawler/src/main/java/com/java/example/tanzu/wherefordinner/model/SearchCriteria.java didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-crawler/src/main/java/com/java/example/tanzu/wherefordinner/resources/LocalRandomSearcher.java didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-crawler/src/main/java/com/java/example/tanzu/wherefordinner/resources/SearchResource.java didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-crawler/src/main/resources/application.properties didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-crawler/src/main/resources/application.yml didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-crawler/src/test/java/com/java/example/tanzu/wherefordinner/WhereForDinnerCrawlerApplicationTests.java didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/.gitignore didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/.mvn/wrapper/maven-wrapper.properties didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/README.md didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/Tiltfile didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/config/workload.yaml didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/mvnw didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/mvnw.cmd didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/pom.xml didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/src/main/java/com/java/example/tanzu/wherefordinner/WhereForDinnerNotifyApplication.java didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/src/main/java/com/java/example/tanzu/wherefordinner/config/EmailMessageConfigProperties.java didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/src/main/java/com/java/example/tanzu/wherefordinner/config/PublisherConfiguration.java didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/src/main/java/com/java/example/tanzu/wherefordinner/functions/AvailabilitySink.java didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/src/main/java/com/java/example/tanzu/wherefordinner/model/Availability.java didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/src/main/java/com/java/example/tanzu/wherefordinner/publisher/EmailPublisher.java didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/src/main/java/com/java/example/tanzu/wherefordinner/publisher/LoggerPublisher.java didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/src/main/java/com/java/example/tanzu/wherefordinner/publisher/Publisher.java didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/src/main/resources/application.yml didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/src/test/java/com/java/example/tanzu/wherefordinner/WhereForDinnerNotifyApplicationTests.java didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/.gitignore didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/.mvn/wrapper/maven-wrapper.properties didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/README.md didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/Tiltfile didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/catalog-info.yaml didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/config/workload.yaml didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/mvnw didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/mvnw.cmd didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/pom.xml didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/main/java/com/java/example/tanzu/wherefordinner/WhereForDinnerResApplication.java didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/main/java/com/java/example/tanzu/wherefordinner/config/OAuth2BindingsPropertiesProcessor.java didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/main/java/com/java/example/tanzu/wherefordinner/config/WebSecurityConfig.java didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/main/java/com/java/example/tanzu/wherefordinner/entity/Search.java didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/main/java/com/java/example/tanzu/wherefordinner/functions/SearchSupplier.java didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/main/java/com/java/example/tanzu/wherefordinner/repository/SearchRepository.java didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/main/java/com/java/example/tanzu/wherefordinner/resources/SearchResource.java didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/main/resources/META-INF/spring.factories didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/main/resources/application.yml didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/main/resources/schema-h2.sql didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/main/resources/schema-mysql.sql didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/main/resources/schema-postgresql.sql didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/test/java/com/java/example/tanzu/wherefordinner/SpringBaseTest.java didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/test/java/com/java/example/tanzu/wherefordinner/WhereForDinnerResApplicationTests.java didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/test/java/com/java/example/tanzu/wherefordinner/repository/SearchRepositoryTest.java didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/test/resources/application.yml didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/.gitignore didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/.mvn/wrapper/maven-wrapper.properties didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/README.md didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/Tiltfile didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/config/workload.yaml didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/mvnw didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/mvnw.cmd didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/pom.xml didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/src/main/java/com/java/example/tanzu/wherefordinner/WhereForDinnerSearchProcApplication.java didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/src/main/java/com/java/example/tanzu/wherefordinner/config/StaticDiningAvailability.java didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/src/main/java/com/java/example/tanzu/wherefordinner/feign/CrawlerClient.java didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/src/main/java/com/java/example/tanzu/wherefordinner/functions/Search.java didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/src/main/java/com/java/example/tanzu/wherefordinner/model/Availability.java didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/src/main/java/com/java/example/tanzu/wherefordinner/model/SearchCriteria.java didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/src/main/java/com/java/example/tanzu/wherefordinner/processor/SearchProcessor.java didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/src/main/java/com/java/example/tanzu/wherefordinner/processor/cache/HashCache.java didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/src/main/java/com/java/example/tanzu/wherefordinner/processor/cache/MemoryHashCache.java didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/src/main/java/com/java/example/tanzu/wherefordinner/processor/cache/RedisHashCache.java didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/src/main/java/com/java/example/tanzu/wherefordinner/searcher/Searcher.java didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/src/main/java/com/java/example/tanzu/wherefordinner/searcher/impl/CrawlerSearcher.java didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/src/main/java/com/java/example/tanzu/wherefordinner/searcher/impl/LocalRandomSearcher.java didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/src/main/resources/application.yml didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/src/test/java/com/java/example/tanzu/wherefordinner/WhereForDinnerSearchProcApplicationTests.java didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/.gitignore didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/README.md didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/httpproxy.yaml didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/package-lock.json didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/package.json didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/public/favicon.png didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/public/index.html didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/public/manifest.json didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/public/robots.txt didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/src/App.css didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/src/App.js didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/src/App.test.js didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/src/Availability.js didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/src/DiningNames.js didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/src/DiningSearch.js didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/src/DiningSearches.js didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/src/DiningTypes.js didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/src/SearchDefForm.js didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/src/TimeWindow.js didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/src/images/delete.png didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/src/index.css didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/src/index.js didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/src/logo.svg didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/src/reportWebVitals.js didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┗ Debug where-for-dinner-ui/src/setupTests.js didn't match [**/rmqCluster.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].sources[2].delegate.transformations[1] (YTT)
┃ ┃ ┃ ┃ ┃ ┃ Debug Wrote values file with json content:   {"bsGitBranch":"main","artifactVersion":"0.0.1-beta","bsGitRepository":"github.com?owner=igodwin&repo=where-for-dinner","dbName":"db-where-for-dinner","dbType":"mysql","rabbitMQName":"rmq-where-for-dinner","enableCloudEvents":false,"enableSecurity":false,"cacheName":"cache-where-for-dinner","numRabbitMQClusterNodes":1,"artifactId":"where-for-dinner","serviceNamespace":"service-instances","projectName":"where-for-dinner","workloadNamespace":"workloads","cacheType":"redisCache"}
┃ ┃ ┃ ┃ ┃ ┗  Info Shelling out to YTT with args: [ytt, -f, /tmp/ytt-input7887009188009117357, --data-values-file, /tmp/accelerator-options13907891223326209583.json, --output-files, /tmp/ytt-output16586638094068048617]
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].sources[2].delegate.transformations[2] (RewritePath)
┃ ┃ ┃ ┃ ┗ ┗ Debug Path 'templates/rmqCluster.yaml' matched 'templates/rmqCluster.yaml' with groups {g0=templates/rmqCluster.yaml} and was rewritten to 'config/service-operator/rmqCluster.yaml'
┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].sources[3] (Combo)
┃ ┃ ┃ ┃ ┃  Info Condition (#dbType == 'mysql') evaluated to true
┃ ┃ ┃ ┃ ┃  Info Combo running as Chain
┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.delegate.transformations[0].sources[3].delegate (Chain)
┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, YTT, RewritePath)
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].sources[3].delegate.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃  Info Will include [**/mysqlInstance.yaml]
┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/components/where-for-dinner-api-gateway/where-for-dinner-api-gateway.yaml didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/components/where-for-dinner-availability/where-for-dinner-availability.yaml didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/components/where-for-dinner-notify/where-for-dinner-notify.yaml didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/components/where-for-dinner-search/where-for-dinner-search.yaml didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/components/where-for-dinner-search-proc/where-for-dinner-search-proc.yaml didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/components/where-for-dinner-ui/where-for-dinner-ui.yaml didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/groups/org.yaml didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/resources/db/where-for-dinner-db-resource.yaml didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/resources/messaging/where-for-dinner-messaging-resource.yaml didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/systems/where-for-dinner-system.yaml didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug doc/TAPDeployment.md didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug doc/images/AppHomeScreen.png didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug doc/images/DinnerHighLevelArch.png didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug doc/images/KnativeEventing.png didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug doc/images/SCSMessaging.png didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug icons/where-for-dinner.png didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug templates/appSSOInstance.yaml didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug templates/clientRegistrationResourceClaim.yaml didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug templates/knEventing.yaml didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug templates/mysqlInstance.yaml matched [**/mysqlInstance.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug templates/mysqlResourceClaim.yaml didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug templates/redisInstance.yaml didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug templates/redisResourceClaim.yaml didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug templates/rmqCluster.yaml didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug templates/rmqResourceClaim.yaml didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug templates/workloads.yaml didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-api-gateway/.gitignore didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-api-gateway/Tiltfile didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-api-gateway/config/workload.yaml didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-api-gateway/pom.xml didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-api-gateway/src/main/java/com/java/example/tanzu/wherefordinner/DinnerAPIGatewayApplication.java didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-api-gateway/src/main/resources/application.yaml didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/.gitignore didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/.mvn/wrapper/maven-wrapper.properties didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/Tiltfile didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/config/workload.yaml didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/mvnw didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/mvnw.cmd didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/pom.xml didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/main/java/com/java/example/tanzu/wherefordinner/WhereForDinnerAvailabilityApplication.java didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/main/java/com/java/example/tanzu/wherefordinner/config/OAuth2BindingsPropertiesProcessor.java didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/main/java/com/java/example/tanzu/wherefordinner/config/WebSecurityConfig.java didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/main/java/com/java/example/tanzu/wherefordinner/entity/Availability.java didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/main/java/com/java/example/tanzu/wherefordinner/entity/AvailabilityWindow.java didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/main/java/com/java/example/tanzu/wherefordinner/function/AvailabilitySink.java didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/main/java/com/java/example/tanzu/wherefordinner/model/Availability.java didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/main/java/com/java/example/tanzu/wherefordinner/repository/AvailabilityRepository.java didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/main/java/com/java/example/tanzu/wherefordinner/repository/AvailabilityWindowRepository.java didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/main/java/com/java/example/tanzu/wherefordinner/resources/AvailabilityResource.java didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/main/resources/META-INF/spring.factories didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/main/resources/application.yaml didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/main/resources/schema-h2.sql didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/main/resources/schema-mysql.sql didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/main/resources/schema-postgresql.sql didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/test/java/com/java/example/tanzu/wherefordinner/WhereForDinnerAvailabilityApplicationTests.java didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-crawler/.gitignore didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-crawler/.mvn/wrapper/maven-wrapper.properties didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-crawler/config/workload.yaml didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-crawler/mvnw didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-crawler/mvnw.cmd didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-crawler/pom.xml didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-crawler/src/main/java/com/java/example/tanzu/wherefordinner/WhereForDinnerCrawlerApplication.java didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-crawler/src/main/java/com/java/example/tanzu/wherefordinner/config/StaticDiningAvailability.java didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-crawler/src/main/java/com/java/example/tanzu/wherefordinner/model/Availability.java didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-crawler/src/main/java/com/java/example/tanzu/wherefordinner/model/SearchCriteria.java didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-crawler/src/main/java/com/java/example/tanzu/wherefordinner/resources/LocalRandomSearcher.java didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-crawler/src/main/java/com/java/example/tanzu/wherefordinner/resources/SearchResource.java didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-crawler/src/main/resources/application.properties didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-crawler/src/main/resources/application.yml didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-crawler/src/test/java/com/java/example/tanzu/wherefordinner/WhereForDinnerCrawlerApplicationTests.java didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/.gitignore didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/.mvn/wrapper/maven-wrapper.properties didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/README.md didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/Tiltfile didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/config/workload.yaml didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/mvnw didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/mvnw.cmd didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/pom.xml didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/src/main/java/com/java/example/tanzu/wherefordinner/WhereForDinnerNotifyApplication.java didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/src/main/java/com/java/example/tanzu/wherefordinner/config/EmailMessageConfigProperties.java didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/src/main/java/com/java/example/tanzu/wherefordinner/config/PublisherConfiguration.java didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/src/main/java/com/java/example/tanzu/wherefordinner/functions/AvailabilitySink.java didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/src/main/java/com/java/example/tanzu/wherefordinner/model/Availability.java didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/src/main/java/com/java/example/tanzu/wherefordinner/publisher/EmailPublisher.java didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/src/main/java/com/java/example/tanzu/wherefordinner/publisher/LoggerPublisher.java didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/src/main/java/com/java/example/tanzu/wherefordinner/publisher/Publisher.java didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/src/main/resources/application.yml didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/src/test/java/com/java/example/tanzu/wherefordinner/WhereForDinnerNotifyApplicationTests.java didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/.gitignore didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/.mvn/wrapper/maven-wrapper.properties didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/README.md didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/Tiltfile didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/catalog-info.yaml didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/config/workload.yaml didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/mvnw didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/mvnw.cmd didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/pom.xml didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/main/java/com/java/example/tanzu/wherefordinner/WhereForDinnerResApplication.java didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/main/java/com/java/example/tanzu/wherefordinner/config/OAuth2BindingsPropertiesProcessor.java didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/main/java/com/java/example/tanzu/wherefordinner/config/WebSecurityConfig.java didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/main/java/com/java/example/tanzu/wherefordinner/entity/Search.java didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/main/java/com/java/example/tanzu/wherefordinner/functions/SearchSupplier.java didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/main/java/com/java/example/tanzu/wherefordinner/repository/SearchRepository.java didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/main/java/com/java/example/tanzu/wherefordinner/resources/SearchResource.java didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/main/resources/META-INF/spring.factories didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/main/resources/application.yml didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/main/resources/schema-h2.sql didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/main/resources/schema-mysql.sql didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/main/resources/schema-postgresql.sql didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/test/java/com/java/example/tanzu/wherefordinner/SpringBaseTest.java didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/test/java/com/java/example/tanzu/wherefordinner/WhereForDinnerResApplicationTests.java didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/test/java/com/java/example/tanzu/wherefordinner/repository/SearchRepositoryTest.java didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/test/resources/application.yml didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/.gitignore didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/.mvn/wrapper/maven-wrapper.properties didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/README.md didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/Tiltfile didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/config/workload.yaml didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/mvnw didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/mvnw.cmd didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/pom.xml didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/src/main/java/com/java/example/tanzu/wherefordinner/WhereForDinnerSearchProcApplication.java didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/src/main/java/com/java/example/tanzu/wherefordinner/config/StaticDiningAvailability.java didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/src/main/java/com/java/example/tanzu/wherefordinner/feign/CrawlerClient.java didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/src/main/java/com/java/example/tanzu/wherefordinner/functions/Search.java didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/src/main/java/com/java/example/tanzu/wherefordinner/model/Availability.java didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/src/main/java/com/java/example/tanzu/wherefordinner/model/SearchCriteria.java didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/src/main/java/com/java/example/tanzu/wherefordinner/processor/SearchProcessor.java didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/src/main/java/com/java/example/tanzu/wherefordinner/processor/cache/HashCache.java didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/src/main/java/com/java/example/tanzu/wherefordinner/processor/cache/MemoryHashCache.java didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/src/main/java/com/java/example/tanzu/wherefordinner/processor/cache/RedisHashCache.java didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/src/main/java/com/java/example/tanzu/wherefordinner/searcher/Searcher.java didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/src/main/java/com/java/example/tanzu/wherefordinner/searcher/impl/CrawlerSearcher.java didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/src/main/java/com/java/example/tanzu/wherefordinner/searcher/impl/LocalRandomSearcher.java didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/src/main/resources/application.yml didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/src/test/java/com/java/example/tanzu/wherefordinner/WhereForDinnerSearchProcApplicationTests.java didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/.gitignore didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/README.md didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/httpproxy.yaml didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/package-lock.json didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/package.json didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/public/favicon.png didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/public/index.html didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/public/manifest.json didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/public/robots.txt didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/src/App.css didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/src/App.js didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/src/App.test.js didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/src/Availability.js didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/src/DiningNames.js didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/src/DiningSearch.js didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/src/DiningSearches.js didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/src/DiningTypes.js didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/src/SearchDefForm.js didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/src/TimeWindow.js didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/src/images/delete.png didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/src/index.css didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/src/index.js didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/src/logo.svg didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/src/reportWebVitals.js didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┗ Debug where-for-dinner-ui/src/setupTests.js didn't match [**/mysqlInstance.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].sources[3].delegate.transformations[1] (YTT)
┃ ┃ ┃ ┃ ┃ ┃ Debug Wrote values file with json content:   {"bsGitBranch":"main","artifactVersion":"0.0.1-beta","bsGitRepository":"github.com?owner=igodwin&repo=where-for-dinner","dbName":"db-where-for-dinner","dbType":"mysql","rabbitMQName":"rmq-where-for-dinner","enableCloudEvents":false,"enableSecurity":false,"cacheName":"cache-where-for-dinner","numRabbitMQClusterNodes":1,"artifactId":"where-for-dinner","serviceNamespace":"service-instances","projectName":"where-for-dinner","workloadNamespace":"workloads","cacheType":"redisCache"}
┃ ┃ ┃ ┃ ┃ ┗  Info Shelling out to YTT with args: [ytt, -f, /tmp/ytt-input12341994701136481974, --data-values-file, /tmp/accelerator-options6651993524297469931.json, --output-files, /tmp/ytt-output16444913385278920027]
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].sources[3].delegate.transformations[2] (RewritePath)
┃ ┃ ┃ ┃ ┗ ┗ Debug Path 'templates/mysqlInstance.yaml' matched 'templates/mysqlInstance.yaml' with groups {g0=templates/mysqlInstance.yaml} and was rewritten to 'config/service-operator/mysqlInstance.yaml'
┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].sources[4] (Combo)
┃ ┃ ┃ ┃ ┃  Info Combo running as Chain
┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.delegate.transformations[0].sources[4].delegate (Chain)
┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, YTT, RewritePath)
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].sources[4].delegate.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃  Info Will include [**/rmqResourceClaim.yaml]
┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/components/where-for-dinner-api-gateway/where-for-dinner-api-gateway.yaml didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/components/where-for-dinner-availability/where-for-dinner-availability.yaml didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/components/where-for-dinner-notify/where-for-dinner-notify.yaml didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/components/where-for-dinner-search/where-for-dinner-search.yaml didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/components/where-for-dinner-search-proc/where-for-dinner-search-proc.yaml didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/components/where-for-dinner-ui/where-for-dinner-ui.yaml didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/groups/org.yaml didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/resources/db/where-for-dinner-db-resource.yaml didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/resources/messaging/where-for-dinner-messaging-resource.yaml didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/systems/where-for-dinner-system.yaml didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug doc/TAPDeployment.md didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug doc/images/AppHomeScreen.png didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug doc/images/DinnerHighLevelArch.png didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug doc/images/KnativeEventing.png didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug doc/images/SCSMessaging.png didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug icons/where-for-dinner.png didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug templates/appSSOInstance.yaml didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug templates/clientRegistrationResourceClaim.yaml didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug templates/knEventing.yaml didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug templates/mysqlInstance.yaml didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug templates/mysqlResourceClaim.yaml didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug templates/redisInstance.yaml didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug templates/redisResourceClaim.yaml didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug templates/rmqCluster.yaml didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug templates/rmqResourceClaim.yaml matched [**/rmqResourceClaim.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug templates/workloads.yaml didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-api-gateway/.gitignore didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-api-gateway/Tiltfile didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-api-gateway/config/workload.yaml didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-api-gateway/pom.xml didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-api-gateway/src/main/java/com/java/example/tanzu/wherefordinner/DinnerAPIGatewayApplication.java didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-api-gateway/src/main/resources/application.yaml didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/.gitignore didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/.mvn/wrapper/maven-wrapper.properties didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/Tiltfile didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/config/workload.yaml didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/mvnw didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/mvnw.cmd didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/pom.xml didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/main/java/com/java/example/tanzu/wherefordinner/WhereForDinnerAvailabilityApplication.java didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/main/java/com/java/example/tanzu/wherefordinner/config/OAuth2BindingsPropertiesProcessor.java didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/main/java/com/java/example/tanzu/wherefordinner/config/WebSecurityConfig.java didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/main/java/com/java/example/tanzu/wherefordinner/entity/Availability.java didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/main/java/com/java/example/tanzu/wherefordinner/entity/AvailabilityWindow.java didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/main/java/com/java/example/tanzu/wherefordinner/function/AvailabilitySink.java didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/main/java/com/java/example/tanzu/wherefordinner/model/Availability.java didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/main/java/com/java/example/tanzu/wherefordinner/repository/AvailabilityRepository.java didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/main/java/com/java/example/tanzu/wherefordinner/repository/AvailabilityWindowRepository.java didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/main/java/com/java/example/tanzu/wherefordinner/resources/AvailabilityResource.java didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/main/resources/META-INF/spring.factories didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/main/resources/application.yaml didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/main/resources/schema-h2.sql didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/main/resources/schema-mysql.sql didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/main/resources/schema-postgresql.sql didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/test/java/com/java/example/tanzu/wherefordinner/WhereForDinnerAvailabilityApplicationTests.java didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-crawler/.gitignore didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-crawler/.mvn/wrapper/maven-wrapper.properties didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-crawler/config/workload.yaml didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-crawler/mvnw didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-crawler/mvnw.cmd didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-crawler/pom.xml didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-crawler/src/main/java/com/java/example/tanzu/wherefordinner/WhereForDinnerCrawlerApplication.java didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-crawler/src/main/java/com/java/example/tanzu/wherefordinner/config/StaticDiningAvailability.java didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-crawler/src/main/java/com/java/example/tanzu/wherefordinner/model/Availability.java didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-crawler/src/main/java/com/java/example/tanzu/wherefordinner/model/SearchCriteria.java didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-crawler/src/main/java/com/java/example/tanzu/wherefordinner/resources/LocalRandomSearcher.java didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-crawler/src/main/java/com/java/example/tanzu/wherefordinner/resources/SearchResource.java didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-crawler/src/main/resources/application.properties didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-crawler/src/main/resources/application.yml didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-crawler/src/test/java/com/java/example/tanzu/wherefordinner/WhereForDinnerCrawlerApplicationTests.java didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/.gitignore didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/.mvn/wrapper/maven-wrapper.properties didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/README.md didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/Tiltfile didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/config/workload.yaml didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/mvnw didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/mvnw.cmd didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/pom.xml didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/src/main/java/com/java/example/tanzu/wherefordinner/WhereForDinnerNotifyApplication.java didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/src/main/java/com/java/example/tanzu/wherefordinner/config/EmailMessageConfigProperties.java didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/src/main/java/com/java/example/tanzu/wherefordinner/config/PublisherConfiguration.java didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/src/main/java/com/java/example/tanzu/wherefordinner/functions/AvailabilitySink.java didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/src/main/java/com/java/example/tanzu/wherefordinner/model/Availability.java didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/src/main/java/com/java/example/tanzu/wherefordinner/publisher/EmailPublisher.java didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/src/main/java/com/java/example/tanzu/wherefordinner/publisher/LoggerPublisher.java didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/src/main/java/com/java/example/tanzu/wherefordinner/publisher/Publisher.java didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/src/main/resources/application.yml didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/src/test/java/com/java/example/tanzu/wherefordinner/WhereForDinnerNotifyApplicationTests.java didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/.gitignore didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/.mvn/wrapper/maven-wrapper.properties didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/README.md didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/Tiltfile didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/catalog-info.yaml didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/config/workload.yaml didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/mvnw didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/mvnw.cmd didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/pom.xml didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/main/java/com/java/example/tanzu/wherefordinner/WhereForDinnerResApplication.java didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/main/java/com/java/example/tanzu/wherefordinner/config/OAuth2BindingsPropertiesProcessor.java didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/main/java/com/java/example/tanzu/wherefordinner/config/WebSecurityConfig.java didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/main/java/com/java/example/tanzu/wherefordinner/entity/Search.java didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/main/java/com/java/example/tanzu/wherefordinner/functions/SearchSupplier.java didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/main/java/com/java/example/tanzu/wherefordinner/repository/SearchRepository.java didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/main/java/com/java/example/tanzu/wherefordinner/resources/SearchResource.java didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/main/resources/META-INF/spring.factories didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/main/resources/application.yml didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/main/resources/schema-h2.sql didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/main/resources/schema-mysql.sql didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/main/resources/schema-postgresql.sql didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/test/java/com/java/example/tanzu/wherefordinner/SpringBaseTest.java didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/test/java/com/java/example/tanzu/wherefordinner/WhereForDinnerResApplicationTests.java didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/test/java/com/java/example/tanzu/wherefordinner/repository/SearchRepositoryTest.java didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/test/resources/application.yml didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/.gitignore didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/.mvn/wrapper/maven-wrapper.properties didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/README.md didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/Tiltfile didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/config/workload.yaml didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/mvnw didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/mvnw.cmd didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/pom.xml didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/src/main/java/com/java/example/tanzu/wherefordinner/WhereForDinnerSearchProcApplication.java didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/src/main/java/com/java/example/tanzu/wherefordinner/config/StaticDiningAvailability.java didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/src/main/java/com/java/example/tanzu/wherefordinner/feign/CrawlerClient.java didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/src/main/java/com/java/example/tanzu/wherefordinner/functions/Search.java didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/src/main/java/com/java/example/tanzu/wherefordinner/model/Availability.java didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/src/main/java/com/java/example/tanzu/wherefordinner/model/SearchCriteria.java didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/src/main/java/com/java/example/tanzu/wherefordinner/processor/SearchProcessor.java didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/src/main/java/com/java/example/tanzu/wherefordinner/processor/cache/HashCache.java didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/src/main/java/com/java/example/tanzu/wherefordinner/processor/cache/MemoryHashCache.java didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/src/main/java/com/java/example/tanzu/wherefordinner/processor/cache/RedisHashCache.java didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/src/main/java/com/java/example/tanzu/wherefordinner/searcher/Searcher.java didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/src/main/java/com/java/example/tanzu/wherefordinner/searcher/impl/CrawlerSearcher.java didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/src/main/java/com/java/example/tanzu/wherefordinner/searcher/impl/LocalRandomSearcher.java didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/src/main/resources/application.yml didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/src/test/java/com/java/example/tanzu/wherefordinner/WhereForDinnerSearchProcApplicationTests.java didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/.gitignore didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/README.md didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/httpproxy.yaml didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/package-lock.json didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/package.json didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/public/favicon.png didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/public/index.html didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/public/manifest.json didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/public/robots.txt didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/src/App.css didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/src/App.js didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/src/App.test.js didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/src/Availability.js didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/src/DiningNames.js didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/src/DiningSearch.js didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/src/DiningSearches.js didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/src/DiningTypes.js didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/src/SearchDefForm.js didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/src/TimeWindow.js didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/src/images/delete.png didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/src/index.css didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/src/index.js didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/src/logo.svg didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/src/reportWebVitals.js didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┗ Debug where-for-dinner-ui/src/setupTests.js didn't match [**/rmqResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].sources[4].delegate.transformations[1] (YTT)
┃ ┃ ┃ ┃ ┃ ┃ Debug Wrote values file with json content:   {"bsGitBranch":"main","artifactVersion":"0.0.1-beta","bsGitRepository":"github.com?owner=igodwin&repo=where-for-dinner","dbName":"db-where-for-dinner","dbType":"mysql","rabbitMQName":"rmq-where-for-dinner","enableCloudEvents":false,"enableSecurity":false,"cacheName":"cache-where-for-dinner","numRabbitMQClusterNodes":1,"artifactId":"where-for-dinner","serviceNamespace":"service-instances","projectName":"where-for-dinner","workloadNamespace":"workloads","cacheType":"redisCache"}
┃ ┃ ┃ ┃ ┃ ┗  Info Shelling out to YTT with args: [ytt, -f, /tmp/ytt-input13617613419992765712, --data-values-file, /tmp/accelerator-options1637671378024449983.json, --output-files, /tmp/ytt-output12502142694235365102]
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].sources[4].delegate.transformations[2] (RewritePath)
┃ ┃ ┃ ┃ ┗ ┗ Debug Path 'templates/rmqResourceClaim.yaml' matched 'templates/rmqResourceClaim.yaml' with groups {g0=templates/rmqResourceClaim.yaml} and was rewritten to 'config/app-operator/rmqResourceClaim.yaml'
┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].sources[5] (Combo)
┃ ┃ ┃ ┃ ┃  Info Condition (#dbType == 'mysql') evaluated to true
┃ ┃ ┃ ┃ ┃  Info Combo running as Chain
┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.delegate.transformations[0].sources[5].delegate (Chain)
┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, YTT, RewritePath)
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].sources[5].delegate.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃  Info Will include [**/mysqlResourceClaim.yaml]
┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/components/where-for-dinner-api-gateway/where-for-dinner-api-gateway.yaml didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/components/where-for-dinner-availability/where-for-dinner-availability.yaml didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/components/where-for-dinner-notify/where-for-dinner-notify.yaml didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/components/where-for-dinner-search/where-for-dinner-search.yaml didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/components/where-for-dinner-search-proc/where-for-dinner-search-proc.yaml didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/components/where-for-dinner-ui/where-for-dinner-ui.yaml didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/groups/org.yaml didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/resources/db/where-for-dinner-db-resource.yaml didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/resources/messaging/where-for-dinner-messaging-resource.yaml didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/systems/where-for-dinner-system.yaml didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug doc/TAPDeployment.md didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug doc/images/AppHomeScreen.png didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug doc/images/DinnerHighLevelArch.png didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug doc/images/KnativeEventing.png didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug doc/images/SCSMessaging.png didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug icons/where-for-dinner.png didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug templates/appSSOInstance.yaml didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug templates/clientRegistrationResourceClaim.yaml didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug templates/knEventing.yaml didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug templates/mysqlInstance.yaml didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug templates/mysqlResourceClaim.yaml matched [**/mysqlResourceClaim.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug templates/redisInstance.yaml didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug templates/redisResourceClaim.yaml didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug templates/rmqCluster.yaml didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug templates/rmqResourceClaim.yaml didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug templates/workloads.yaml didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-api-gateway/.gitignore didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-api-gateway/Tiltfile didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-api-gateway/config/workload.yaml didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-api-gateway/pom.xml didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-api-gateway/src/main/java/com/java/example/tanzu/wherefordinner/DinnerAPIGatewayApplication.java didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-api-gateway/src/main/resources/application.yaml didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/.gitignore didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/.mvn/wrapper/maven-wrapper.properties didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/Tiltfile didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/config/workload.yaml didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/mvnw didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/mvnw.cmd didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/pom.xml didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/main/java/com/java/example/tanzu/wherefordinner/WhereForDinnerAvailabilityApplication.java didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/main/java/com/java/example/tanzu/wherefordinner/config/OAuth2BindingsPropertiesProcessor.java didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/main/java/com/java/example/tanzu/wherefordinner/config/WebSecurityConfig.java didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/main/java/com/java/example/tanzu/wherefordinner/entity/Availability.java didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/main/java/com/java/example/tanzu/wherefordinner/entity/AvailabilityWindow.java didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/main/java/com/java/example/tanzu/wherefordinner/function/AvailabilitySink.java didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/main/java/com/java/example/tanzu/wherefordinner/model/Availability.java didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/main/java/com/java/example/tanzu/wherefordinner/repository/AvailabilityRepository.java didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/main/java/com/java/example/tanzu/wherefordinner/repository/AvailabilityWindowRepository.java didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/main/java/com/java/example/tanzu/wherefordinner/resources/AvailabilityResource.java didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/main/resources/META-INF/spring.factories didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/main/resources/application.yaml didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/main/resources/schema-h2.sql didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/main/resources/schema-mysql.sql didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/main/resources/schema-postgresql.sql didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/test/java/com/java/example/tanzu/wherefordinner/WhereForDinnerAvailabilityApplicationTests.java didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-crawler/.gitignore didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-crawler/.mvn/wrapper/maven-wrapper.properties didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-crawler/config/workload.yaml didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-crawler/mvnw didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-crawler/mvnw.cmd didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-crawler/pom.xml didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-crawler/src/main/java/com/java/example/tanzu/wherefordinner/WhereForDinnerCrawlerApplication.java didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-crawler/src/main/java/com/java/example/tanzu/wherefordinner/config/StaticDiningAvailability.java didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-crawler/src/main/java/com/java/example/tanzu/wherefordinner/model/Availability.java didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-crawler/src/main/java/com/java/example/tanzu/wherefordinner/model/SearchCriteria.java didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-crawler/src/main/java/com/java/example/tanzu/wherefordinner/resources/LocalRandomSearcher.java didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-crawler/src/main/java/com/java/example/tanzu/wherefordinner/resources/SearchResource.java didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-crawler/src/main/resources/application.properties didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-crawler/src/main/resources/application.yml didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-crawler/src/test/java/com/java/example/tanzu/wherefordinner/WhereForDinnerCrawlerApplicationTests.java didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/.gitignore didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/.mvn/wrapper/maven-wrapper.properties didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/README.md didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/Tiltfile didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/config/workload.yaml didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/mvnw didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/mvnw.cmd didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/pom.xml didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/src/main/java/com/java/example/tanzu/wherefordinner/WhereForDinnerNotifyApplication.java didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/src/main/java/com/java/example/tanzu/wherefordinner/config/EmailMessageConfigProperties.java didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/src/main/java/com/java/example/tanzu/wherefordinner/config/PublisherConfiguration.java didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/src/main/java/com/java/example/tanzu/wherefordinner/functions/AvailabilitySink.java didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/src/main/java/com/java/example/tanzu/wherefordinner/model/Availability.java didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/src/main/java/com/java/example/tanzu/wherefordinner/publisher/EmailPublisher.java didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/src/main/java/com/java/example/tanzu/wherefordinner/publisher/LoggerPublisher.java didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/src/main/java/com/java/example/tanzu/wherefordinner/publisher/Publisher.java didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/src/main/resources/application.yml didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/src/test/java/com/java/example/tanzu/wherefordinner/WhereForDinnerNotifyApplicationTests.java didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/.gitignore didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/.mvn/wrapper/maven-wrapper.properties didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/README.md didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/Tiltfile didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/catalog-info.yaml didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/config/workload.yaml didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/mvnw didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/mvnw.cmd didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/pom.xml didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/main/java/com/java/example/tanzu/wherefordinner/WhereForDinnerResApplication.java didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/main/java/com/java/example/tanzu/wherefordinner/config/OAuth2BindingsPropertiesProcessor.java didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/main/java/com/java/example/tanzu/wherefordinner/config/WebSecurityConfig.java didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/main/java/com/java/example/tanzu/wherefordinner/entity/Search.java didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/main/java/com/java/example/tanzu/wherefordinner/functions/SearchSupplier.java didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/main/java/com/java/example/tanzu/wherefordinner/repository/SearchRepository.java didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/main/java/com/java/example/tanzu/wherefordinner/resources/SearchResource.java didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/main/resources/META-INF/spring.factories didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/main/resources/application.yml didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/main/resources/schema-h2.sql didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/main/resources/schema-mysql.sql didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/main/resources/schema-postgresql.sql didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/test/java/com/java/example/tanzu/wherefordinner/SpringBaseTest.java didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/test/java/com/java/example/tanzu/wherefordinner/WhereForDinnerResApplicationTests.java didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/test/java/com/java/example/tanzu/wherefordinner/repository/SearchRepositoryTest.java didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/test/resources/application.yml didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/.gitignore didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/.mvn/wrapper/maven-wrapper.properties didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/README.md didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/Tiltfile didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/config/workload.yaml didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/mvnw didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/mvnw.cmd didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/pom.xml didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/src/main/java/com/java/example/tanzu/wherefordinner/WhereForDinnerSearchProcApplication.java didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/src/main/java/com/java/example/tanzu/wherefordinner/config/StaticDiningAvailability.java didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/src/main/java/com/java/example/tanzu/wherefordinner/feign/CrawlerClient.java didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/src/main/java/com/java/example/tanzu/wherefordinner/functions/Search.java didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/src/main/java/com/java/example/tanzu/wherefordinner/model/Availability.java didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/src/main/java/com/java/example/tanzu/wherefordinner/model/SearchCriteria.java didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/src/main/java/com/java/example/tanzu/wherefordinner/processor/SearchProcessor.java didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/src/main/java/com/java/example/tanzu/wherefordinner/processor/cache/HashCache.java didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/src/main/java/com/java/example/tanzu/wherefordinner/processor/cache/MemoryHashCache.java didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/src/main/java/com/java/example/tanzu/wherefordinner/processor/cache/RedisHashCache.java didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/src/main/java/com/java/example/tanzu/wherefordinner/searcher/Searcher.java didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/src/main/java/com/java/example/tanzu/wherefordinner/searcher/impl/CrawlerSearcher.java didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/src/main/java/com/java/example/tanzu/wherefordinner/searcher/impl/LocalRandomSearcher.java didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/src/main/resources/application.yml didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/src/test/java/com/java/example/tanzu/wherefordinner/WhereForDinnerSearchProcApplicationTests.java didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/.gitignore didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/README.md didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/httpproxy.yaml didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/package-lock.json didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/package.json didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/public/favicon.png didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/public/index.html didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/public/manifest.json didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/public/robots.txt didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/src/App.css didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/src/App.js didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/src/App.test.js didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/src/Availability.js didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/src/DiningNames.js didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/src/DiningSearch.js didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/src/DiningSearches.js didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/src/DiningTypes.js didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/src/SearchDefForm.js didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/src/TimeWindow.js didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/src/images/delete.png didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/src/index.css didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/src/index.js didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/src/logo.svg didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/src/reportWebVitals.js didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┗ Debug where-for-dinner-ui/src/setupTests.js didn't match [**/mysqlResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].sources[5].delegate.transformations[1] (YTT)
┃ ┃ ┃ ┃ ┃ ┃ Debug Wrote values file with json content:   {"bsGitBranch":"main","artifactVersion":"0.0.1-beta","bsGitRepository":"github.com?owner=igodwin&repo=where-for-dinner","dbName":"db-where-for-dinner","dbType":"mysql","rabbitMQName":"rmq-where-for-dinner","enableCloudEvents":false,"enableSecurity":false,"cacheName":"cache-where-for-dinner","numRabbitMQClusterNodes":1,"artifactId":"where-for-dinner","serviceNamespace":"service-instances","projectName":"where-for-dinner","workloadNamespace":"workloads","cacheType":"redisCache"}
┃ ┃ ┃ ┃ ┃ ┗  Info Shelling out to YTT with args: [ytt, -f, /tmp/ytt-input16850480478897462001, --data-values-file, /tmp/accelerator-options10854807282490050784.json, --output-files, /tmp/ytt-output8037713922264376417]
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].sources[5].delegate.transformations[2] (RewritePath)
┃ ┃ ┃ ┃ ┗ ┗ Debug Path 'templates/mysqlResourceClaim.yaml' matched 'templates/mysqlResourceClaim.yaml' with groups {g0=templates/mysqlResourceClaim.yaml} and was rewritten to 'config/app-operator/mysqlResourceClaim.yaml'
┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].sources[6] (Combo)
┃ ┃ ┃ ┃ ┃  Info Condition (#enableCloudEvents) evaluated to false
┃ ┃ ┃ ┃ ┗ null ()
┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].sources[7] (Combo)
┃ ┃ ┃ ┃ ┃  Info Condition (#enableSecurity) evaluated to false
┃ ┃ ┃ ┃ ┗ null ()
┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].sources[8] (Combo)
┃ ┃ ┃ ┃ ┃  Info Condition (#cacheType == 'redisCache') evaluated to true
┃ ┃ ┃ ┃ ┃  Info Combo running as Chain
┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.delegate.transformations[0].sources[8].delegate (Chain)
┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, YTT, RewritePath, RewritePath)
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].sources[8].delegate.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃  Info Will include [**/redisInstance.yaml, **/redisResourceClaim.yaml]
┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/components/where-for-dinner-api-gateway/where-for-dinner-api-gateway.yaml didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/components/where-for-dinner-availability/where-for-dinner-availability.yaml didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/components/where-for-dinner-notify/where-for-dinner-notify.yaml didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/components/where-for-dinner-search/where-for-dinner-search.yaml didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/components/where-for-dinner-search-proc/where-for-dinner-search-proc.yaml didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/components/where-for-dinner-ui/where-for-dinner-ui.yaml didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/groups/org.yaml didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/resources/db/where-for-dinner-db-resource.yaml didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/resources/messaging/where-for-dinner-messaging-resource.yaml didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/systems/where-for-dinner-system.yaml didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug doc/TAPDeployment.md didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug doc/images/AppHomeScreen.png didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug doc/images/DinnerHighLevelArch.png didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug doc/images/KnativeEventing.png didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug doc/images/SCSMessaging.png didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug icons/where-for-dinner.png didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw.cmd didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug templates/appSSOInstance.yaml didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug templates/clientRegistrationResourceClaim.yaml didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug templates/knEventing.yaml didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug templates/mysqlInstance.yaml didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug templates/mysqlResourceClaim.yaml didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug templates/redisInstance.yaml matched [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug templates/redisResourceClaim.yaml matched [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug templates/rmqCluster.yaml didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug templates/rmqResourceClaim.yaml didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug templates/workloads.yaml didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-api-gateway/.gitignore didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-api-gateway/Tiltfile didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-api-gateway/config/workload.yaml didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-api-gateway/pom.xml didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-api-gateway/src/main/java/com/java/example/tanzu/wherefordinner/DinnerAPIGatewayApplication.java didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-api-gateway/src/main/resources/application.yaml didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/.gitignore didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/.mvn/wrapper/maven-wrapper.properties didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/Tiltfile didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/config/workload.yaml didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/mvnw didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/mvnw.cmd didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/pom.xml didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/main/java/com/java/example/tanzu/wherefordinner/WhereForDinnerAvailabilityApplication.java didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/main/java/com/java/example/tanzu/wherefordinner/config/OAuth2BindingsPropertiesProcessor.java didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/main/java/com/java/example/tanzu/wherefordinner/config/WebSecurityConfig.java didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/main/java/com/java/example/tanzu/wherefordinner/entity/Availability.java didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/main/java/com/java/example/tanzu/wherefordinner/entity/AvailabilityWindow.java didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/main/java/com/java/example/tanzu/wherefordinner/function/AvailabilitySink.java didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/main/java/com/java/example/tanzu/wherefordinner/model/Availability.java didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/main/java/com/java/example/tanzu/wherefordinner/repository/AvailabilityRepository.java didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/main/java/com/java/example/tanzu/wherefordinner/repository/AvailabilityWindowRepository.java didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/main/java/com/java/example/tanzu/wherefordinner/resources/AvailabilityResource.java didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/main/resources/META-INF/spring.factories didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/main/resources/application.yaml didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/main/resources/schema-h2.sql didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/main/resources/schema-mysql.sql didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/main/resources/schema-postgresql.sql didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-availability/src/test/java/com/java/example/tanzu/wherefordinner/WhereForDinnerAvailabilityApplicationTests.java didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-crawler/.gitignore didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-crawler/.mvn/wrapper/maven-wrapper.properties didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-crawler/config/workload.yaml didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-crawler/mvnw didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-crawler/mvnw.cmd didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-crawler/pom.xml didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-crawler/src/main/java/com/java/example/tanzu/wherefordinner/WhereForDinnerCrawlerApplication.java didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-crawler/src/main/java/com/java/example/tanzu/wherefordinner/config/StaticDiningAvailability.java didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-crawler/src/main/java/com/java/example/tanzu/wherefordinner/model/Availability.java didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-crawler/src/main/java/com/java/example/tanzu/wherefordinner/model/SearchCriteria.java didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-crawler/src/main/java/com/java/example/tanzu/wherefordinner/resources/LocalRandomSearcher.java didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-crawler/src/main/java/com/java/example/tanzu/wherefordinner/resources/SearchResource.java didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-crawler/src/main/resources/application.properties didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-crawler/src/main/resources/application.yml didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-crawler/src/test/java/com/java/example/tanzu/wherefordinner/WhereForDinnerCrawlerApplicationTests.java didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/.gitignore didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/.mvn/wrapper/maven-wrapper.properties didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/README.md didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/Tiltfile didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/config/workload.yaml didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/mvnw didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/mvnw.cmd didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/pom.xml didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/src/main/java/com/java/example/tanzu/wherefordinner/WhereForDinnerNotifyApplication.java didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/src/main/java/com/java/example/tanzu/wherefordinner/config/EmailMessageConfigProperties.java didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/src/main/java/com/java/example/tanzu/wherefordinner/config/PublisherConfiguration.java didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/src/main/java/com/java/example/tanzu/wherefordinner/functions/AvailabilitySink.java didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/src/main/java/com/java/example/tanzu/wherefordinner/model/Availability.java didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/src/main/java/com/java/example/tanzu/wherefordinner/publisher/EmailPublisher.java didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/src/main/java/com/java/example/tanzu/wherefordinner/publisher/LoggerPublisher.java didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/src/main/java/com/java/example/tanzu/wherefordinner/publisher/Publisher.java didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/src/main/resources/application.yml didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-notify/src/test/java/com/java/example/tanzu/wherefordinner/WhereForDinnerNotifyApplicationTests.java didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/.gitignore didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/.mvn/wrapper/maven-wrapper.properties didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/README.md didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/Tiltfile didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/catalog-info.yaml didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/config/workload.yaml didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/mvnw didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/mvnw.cmd didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/pom.xml didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/main/java/com/java/example/tanzu/wherefordinner/WhereForDinnerResApplication.java didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/main/java/com/java/example/tanzu/wherefordinner/config/OAuth2BindingsPropertiesProcessor.java didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/main/java/com/java/example/tanzu/wherefordinner/config/WebSecurityConfig.java didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/main/java/com/java/example/tanzu/wherefordinner/entity/Search.java didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/main/java/com/java/example/tanzu/wherefordinner/functions/SearchSupplier.java didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/main/java/com/java/example/tanzu/wherefordinner/repository/SearchRepository.java didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/main/java/com/java/example/tanzu/wherefordinner/resources/SearchResource.java didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/main/resources/META-INF/spring.factories didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/main/resources/application.yml didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/main/resources/schema-h2.sql didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/main/resources/schema-mysql.sql didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/main/resources/schema-postgresql.sql didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/test/java/com/java/example/tanzu/wherefordinner/SpringBaseTest.java didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/test/java/com/java/example/tanzu/wherefordinner/WhereForDinnerResApplicationTests.java didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/test/java/com/java/example/tanzu/wherefordinner/repository/SearchRepositoryTest.java didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search/src/test/resources/application.yml didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/.gitignore didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/.mvn/wrapper/maven-wrapper.properties didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/README.md didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/Tiltfile didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/config/workload.yaml didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/mvnw didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/mvnw.cmd didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/pom.xml didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/src/main/java/com/java/example/tanzu/wherefordinner/WhereForDinnerSearchProcApplication.java didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/src/main/java/com/java/example/tanzu/wherefordinner/config/StaticDiningAvailability.java didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/src/main/java/com/java/example/tanzu/wherefordinner/feign/CrawlerClient.java didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/src/main/java/com/java/example/tanzu/wherefordinner/functions/Search.java didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/src/main/java/com/java/example/tanzu/wherefordinner/model/Availability.java didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/src/main/java/com/java/example/tanzu/wherefordinner/model/SearchCriteria.java didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/src/main/java/com/java/example/tanzu/wherefordinner/processor/SearchProcessor.java didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/src/main/java/com/java/example/tanzu/wherefordinner/processor/cache/HashCache.java didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/src/main/java/com/java/example/tanzu/wherefordinner/processor/cache/MemoryHashCache.java didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/src/main/java/com/java/example/tanzu/wherefordinner/processor/cache/RedisHashCache.java didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/src/main/java/com/java/example/tanzu/wherefordinner/searcher/Searcher.java didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/src/main/java/com/java/example/tanzu/wherefordinner/searcher/impl/CrawlerSearcher.java didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/src/main/java/com/java/example/tanzu/wherefordinner/searcher/impl/LocalRandomSearcher.java didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/src/main/resources/application.yml didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-search-proc/src/test/java/com/java/example/tanzu/wherefordinner/WhereForDinnerSearchProcApplicationTests.java didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/.gitignore didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/README.md didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/httpproxy.yaml didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/package-lock.json didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/package.json didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/public/favicon.png didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/public/index.html didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/public/manifest.json didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/public/robots.txt didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/src/App.css didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/src/App.js didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/src/App.test.js didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/src/Availability.js didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/src/DiningNames.js didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/src/DiningSearch.js didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/src/DiningSearches.js didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/src/DiningTypes.js didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/src/SearchDefForm.js didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/src/TimeWindow.js didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/src/images/delete.png didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/src/index.css didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/src/index.js didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/src/logo.svg didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug where-for-dinner-ui/src/reportWebVitals.js didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┗ Debug where-for-dinner-ui/src/setupTests.js didn't match [**/redisInstance.yaml, **/redisResourceClaim.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].sources[8].delegate.transformations[1] (YTT)
┃ ┃ ┃ ┃ ┃ ┃ Debug Wrote values file with json content:   {"bsGitBranch":"main","artifactVersion":"0.0.1-beta","bsGitRepository":"github.com?owner=igodwin&repo=where-for-dinner","dbName":"db-where-for-dinner","dbType":"mysql","rabbitMQName":"rmq-where-for-dinner","enableCloudEvents":false,"enableSecurity":false,"cacheName":"cache-where-for-dinner","numRabbitMQClusterNodes":1,"artifactId":"where-for-dinner","serviceNamespace":"service-instances","projectName":"where-for-dinner","workloadNamespace":"workloads","cacheType":"redisCache"}
┃ ┃ ┃ ┃ ┃ ┗  Info Shelling out to YTT with args: [ytt, -f, /tmp/ytt-input9281404461570725942, --data-values-file, /tmp/accelerator-options12515788619345337749.json, --output-files, /tmp/ytt-output11238835148965597892]
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].sources[8].delegate.transformations[2] (RewritePath)
┃ ┃ ┃ ┃ ┃ ┗ Debug Path 'templates/redisInstance.yaml' matched 'templates/redisInstance.yaml' with groups {g0=templates/redisInstance.yaml} and was rewritten to 'config/service-operator/redisInstance.yaml'
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].sources[8].delegate.transformations[3] (RewritePath)
┃ ┃ ┃ ┗ ┗ ┗ Debug Path 'templates/redisResourceClaim.yaml' matched 'templates/redisResourceClaim.yaml' with groups {g0=templates/redisResourceClaim.yaml} and was rewritten to 'config/app-operator/redisResourceClaim.yaml'
┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[1] (UniquePath)
┃ ┗ ┗ ┗ Debug Multiple representations for path 'README.md', will use the one appearing last 
┗ ╺ engine.transformations[1] (UniquePath)
```
