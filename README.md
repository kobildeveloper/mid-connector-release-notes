## mID Connector v2.3.1

<br/>

**Date** 2021-11-03

### **Docker Download**

### kobil/kobil-cloud-connector:2.3.1  
**DIGEST:** 
### kobil/kobil-cloud-pooler:2.3.1
**DIGEST:** 

<br/>

### **Azurecr Download**
**Connector:** kobilsystems.azurecr.io/idp/ssms-connector:2.3.1  
**Pooler:** kobilsystems.azurecr.io/idp/ssms-pooler:2.3.1
<br/>

------------------------------------
            
### Changed
* Support is added to obtain SHA1 Hash value of Event ID and store in DB for Event Subscription API to reduce key size.
* Connector Client plugins have been released for V1 and V2.
  
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
* MultiTenant:  3.4.1.75470 and 3.5.2.79434
* SingleTenant: 2.8.11.76074
<br/>

### Dependencies
* **Docker Engine 19.03.8**
https://docs.docker.com/engine/release-notes/19.03/
* **Docker Compose 1.28.6**
https://github.com/docker/compose/releases/tag/1.28.6
