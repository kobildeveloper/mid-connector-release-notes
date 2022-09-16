## mID Connector v2.4.2 [NOT RELEASED]

<br/>

**Date** 2022-09-09

### **Docker Download**

### kobil/kobil-cloud-connector:2.4.2
**DIGEST:** 
### kobil/kobil-cloud-pooler:2.4.5
**DIGEST:** 

<br/>

### **Azurecr Download**
- **Connector:** kobilsystems.azurecr.io/idp/ssms-connector:2.4.2  
- **Pooler:** kobilsystems.azurecr.io/idp/ssms-pooler:2.4.5
<br/>

------------------------------------
 
### Changed 
* Updated cloud connector service image version to 2.4.3 which uses the `kobilsystems.azurecr.io/it-solutions/base-images/micro/jre17:1.1.0`
* Updated pooler connector service image version to 2.4.4 which uses the `kobilsystems.azurecr.io/it-solutions/base-images/micro/jre17-idp-pooler:1.1.0`
* core iam image uses kobilsystems.azurecr.io/it-solutions/base-images/micro/jre11-idp-core:1.2.0 micro image as base image
* Updated applogin image version to `1.3.0` which uses the `kobilsystems.azurecr.io/it-solutions/micro/nginx-stable:1.1.0` as base image instead of `bitnami/nginx` image.

## Kobil Core Version: 2.2.0 

### Support Versions
Connector Client plugins: 2.4.2_v1, 2.4.2_v2 
 
### SSMS Version 
* 2.x.x supported 
* 3.x.x supported 

### Tested Server 
* MultiTenant: 3.5.2.79434


### Note
* The vulnerabilities are fixed for all the dependencies of Connector. However, there are vulnerabilities in the base image of java that will be addressed in future releases. 
* Before every deployment, Redis data should be cleared and restarted. 
