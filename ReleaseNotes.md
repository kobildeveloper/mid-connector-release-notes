## mID Connector v2.4.2

<br/>

**Date** 2022-09-16

### **Docker Download**

### kobil/kobil-cloud-connector:2.4.2
**DIGEST:** digest: sha256:078ca92de631cfa5945ee57f6939beb394e932c28145b5b91b3ab2d96bac5996
### kobil/kobil-cloud-pooler:2.4.2
**DIGEST:** sha256:c2fb58237ddaaab920fcae7f8e73d762a5c421523aa3373c3029011da0e95e03

<br/>

### **Azurecr Download**
- **Connector:** kobilsystems.azurecr.io/idp/ssms-connector:2.4.2  
- **Pooler:** kobilsystems.azurecr.io/idp/ssms-pooler:2.4.2
<br/>

------------------------------------
 
### Changed 
* Updated cloud connector service image version to 2.4.3 which uses the `kobilsystems.azurecr.io/it-solutions/base-images/micro/jre17:1.1.0`

* Updated pooler connector service image version to 2.4.4 which uses the `kobilsystems.azurecr.io/it-solutions/base-images/microjre17-idp-pooler:1.1.0`

* Updated mpower connector service image version to 1.9.0 which uses the `gitlab.kobil.com:4567/development/devops/base-images/jre8-micro:1.1.0`

* Updated app login service image version to which uses `gitlab.kobil.com:4567/development/devops/base-images/nginx-stable-micro:1.3.0`

### Note: All these base images will come with less vulnerabilities and only required tools to run the service.

## Kobil Core Version: 2.2.0 

### Support Versions
Connector Client plugins: 2.4.1_v1, 2.4.1_v2 
 
### SSMS Version 
* 2.x.x supported 
* 3.x.x supported 

### Tested Server 
* MultiTenant: 3.4.1.75470 and 3.5.2.79434 
* SingleTenant: 2.8.11.76074 

### Note
* Before every deployment, Redis data should be cleared and restarted. 
