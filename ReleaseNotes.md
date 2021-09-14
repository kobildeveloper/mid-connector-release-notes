## mID Connector v2.3.0

<br/>

**Date** 2021-09-14

### **Docker Download**

### kobil/kobil-cloud-connector:2.3.0  
**DIGEST:** sha256:c494d8b382f3fb51cc17866c56ac8962febcf4a0ea90db703f15fdb73cbd32bb
### kobil/kobil-cloud-pooler:2.3.0
**DIGEST:** sha256:b91e0815a8962444a7275c2f85f9d3d166d192fc75e1d8e9087cc41ce41e68e0

<br/>

### **Azurecr Download**
**Connector:** kobilsystems.azurecr.io/idp/ssms-connector:2.3.0  
**Pooler:** kobilsystems.azurecr.io/idp/ssms-pooler:2.3.0
<br/>

------------------------------------

### Added
* Monitoring SSMS device deletion events is made easier with the new DEVICE_DELETION event, added to the event subscription API.
* Supports Amazon Elasticache.

<br/>

For elasticache support please include below variables

Connector:  
- Environment Variables:  
  - Env Added:
    - ENABLE_REDIS_SSL=true (true for aws redis and false for normal redis)  
  - Env Changed: 
    - DISABLE_CALLBACK_SSL=true (Changed from DISABLE_SSL)
    - REDIS_CLUSTER_MODE=false
    - REDIS_HOST=host:port (Replace your AWS Elasticache host here)
    - REDIS_PWD=password (Replace your AWS Elasticache password here)           
  
Pooler:
- Environment Variables:
  - Env Added:
    - ENABLE_REDIS_SSL=true (true for aws redis and false for normal redis)
  - Env Changed: 
    - DISABLE_CALLBACK_SSL=true (Changed from DISABLE_SSL)
    - REDIS_CLUSTER_MODE=false
    - REDIS_HOST=host:port (Replace your AWS Elasticache host here)
    - REDIS_PWD=password (Replace your AWS Elasticache password here)           
  
### Fixed
* Fixed Elasticache TLS issue
* Fixed SLF4J missing dependency issue
  
<br/>
  
### Not Supported
* Redis sentinal is not supported
<br/>
  
### Kobil Core Version
* 2.1.1
  
<br/>
 
### SSMS Version
* 2.x.x supported
* 3.x.x supported
<br/>

### Tested Server
* MultiTenant: 2.9.0.68478, 3.1.2.71992, 3.4.1.75470 and 3.5.2.79434
* SingleTenant: 2.8.11.76074
<br/>

### Dependencies
* **Docker Engine 19.03.8**
https://docs.docker.com/engine/release-notes/19.03/
* **Docker Compose 1.28.6**
https://github.com/docker/compose/releases/tag/1.28.6
