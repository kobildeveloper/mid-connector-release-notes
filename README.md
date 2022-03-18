## mID Connector v2.4.0

<br/>

**Date** 2022-03-18

### **Docker Download**

### kobil/kobil-cloud-connector:2.4.0
**DIGEST:**  sha256:cc91080bb2388d408ebb556ef06e8bab831eb48c8868f489eb712113352d4ebc
### kobil/kobil-cloud-pooler:2.4.0
**DIGEST:** digest: sha256:288d54293b6ebb1b0b54fa9fc7378e60d75476d61a18ce8293830da041ffd656

<br/>

### **Azurecr Download**
- **Connector:** kobilsystems.azurecr.io/idp/ssms-connector:2.4.0  
- **Pooler:** kobilsystems.azurecr.io/idp/ssms-pooler:2.4.0
<br/>

------------------------------------
            
### Added
* RemoveGlobalPin API - Added a new REST API in ASM management controller to remove the global pin for a user. 
* VerifyOnlineQrNonceResult API – Added a new REST API in ASM service controller to check the nonce login status and additionally get qrValue. It states whether the QR has been scanned and verified successfully or whether the request has been timed out. 
* Dependencies Added in mID connector
  - springdoc-openapi-ui: 1.6.6 

* Dependencies Added in KOBIL UI Extension
  - netty-codec-http: 4.1.72.Final 
  - netty-codec: 4.1.72.Final 
  - httpmime: 4.5.13 
  - saaj-impl: 1.5.3
  - swagger-annotations: 2.1.2
  
### Fixed
* GetDeadEvent API  
  - Scenario fixed: Incorrect/Missing Event Id request
    - Previous: Response code: 400, Status: GENERAL_ERROR 
    - Current: Response Code: 404, Status: NOT_FOUND 
  - Scenario fixed: Transaction related dead device event 
    - Previous: Response code: 400, Status: GENERAL_ERROR (Due to incorrect JSON formatting) 
    - Current: Response code: 200, with proper Event JSON 
 
### Changed 
* Upgraded version 
  - spring boot version: Old - 2.2.6.RELEASE; Current - 2.6.3 
  - Gradle version to v7.4 
  - JDK version from 1.8 to 17 (Compatible with Java 11 too) 
  - Swagger version from 2.0 to 3.0 (Open API) 
  - Removed rt.jar and replaced it with dependencies. 

* Upgraded base image in Docker file 
Image: "adoptopenjdk/openjdk11:jre-11.0.11_9-alpine" -> Image: "openjdk:17.0-jdk-oracle" 
* Upgraded all dependencies to the latest stable version for fixing vulnerabilities. 
*Upgraded dependencies
  - sfm-csv: Old - 3.11; Current - 8.2.3 
  - lombok: Old - 1.18.10; Current - 1.18.22 
  - kotlin-stdlib: Old - 1.3.10; Current - 1.6.10 
  - kotlin-reflect: Old - 1.3.10; Current - 1.6.10 
  - zxing core: Old - 3.3.0; Current - 3.4.1 
  - zxing javase: Old - 3.3.0; Current - 3.4.1 
  - json: Old - 20190722; Current – 20210307 
  - nimbus-jose-jwt: Old - 9.11; Current - 9.15.2 
  - http-mime: Old - 4.5; Current - 4.5.13 
  - jackson-dataformat-properties: Old - 2.10.1; Current - 2.12.5 
  - jackson-databind: Old - 2.10.1; Current - 2.12.5 
  - spring-boot-starter-data-redis: Old - 2.2.6.RELEASE; Current - 2.6.2 
  - jedis: Old - 3.2.0; Current - 3.7.1 
  - saaj-impl: Old - 1.3.4; Current - 1.5.2 
  - okhttp: Old - 4.7.1; Current - 4.9.3 
  - tomcat-embed-el: Old - 9.0.36; Current - 10.0.14 
  - snakeyaml: Old - 1.29; Current - 1.30 
  - netty-handler: Old - 4.1.46.Final; Current - 4.1.72.Final 
  - guava: Old - 30.0-jre; Current - 31.0.1-jre 
  - hibernate-validator: Old - 6.0.20.FInal; Current - 7.0.2.Final 

* The dependencies in the KOBIL UI Extension that are updated to the latest versions are mentioned below: 
  - aws-java-sdk-bom: Old - 1.11.228; Current - 1.12.131 
  - aws-java-sdk: Old - 1.11.381; Current - 1.12.131 
  - lombok: Old - 1.18.10; Current - 1.18.22 
  - nimbus-jose-jwt: Old - 4.11; Current - 9.15.2; 
  - spring-boot-starter-data-redis: Old - 2.2.6.RELEASE; Current - 2.5.7 
  - httpmime: Old - 4.5; Current - 4.5.13 
  - jackson-dataformat-properties: Old - 2.10.1; Current - 2.12.5 
  - jackson-databind: Old - 2.10.1; Current - 2.12.5 
  - jedis: Old - 3.2.0; Current: - 3.7.1 

### Deprecated 

* Dependencies removed in mIDConnector: 
  - springfox-swagger2: 2.9.2 
  - springfox-swagger-ui: 2.9.2 
  - slf4j-nop: 1.7.30 

* Dependencies removed in KOBIL UI Extension: 
  - nimbus-jose-jwt: 9.11 
  - httpclient: 4.5 
  - httpcore: 4.4.1 
  
<br/>

### Kobil Core Version 2.2.0 

### Support Versions
Connector Client plugins: 2.4.0_v1, 2.4.0_v2 
 
### SSMS Version 
2.x.x supported 
3.x.x supported 

### Tested Server 
* MultiTenant: 3.4.1.75470 , 3.5.2.79434 and 3.6.1.81437 
* SingleTenant: 2.8.11.76074 

###Note: 

* The vulnerabilities are fixed for all the dependencies of Connector. However, there are vulnerabilities in the base image of java that will be addressed in future releases. 

* Before every deployment, Redis data should be cleared and restarted.
