## mID Connector v2.3.1

<br/>

**Date** 2021-11-03

### **Docker Download**

### kobil/kobil-cloud-connector:2.3.1  
**DIGEST:** sha256:d53959d11ec03931df71c0f981039895f2c29d18c64338462902f72eca325cb0
### kobil/kobil-cloud-pooler:2.3.0
**DIGEST:** sha256:b91e0815a8962444a7275c2f85f9d3d166d192fc75e1d8e9087cc41ce41e68e0

<br/>

### **Azurecr Download**
**Connector:** kobilsystems.azurecr.io/idp/ssms-connector:2.3.1  
**Pooler:** kobilsystems.azurecr.io/idp/ssms-pooler:2.3.0
<br/>

------------------------------------
            
### Changed
* Support is added to obtain SHA1 Hash value of Event ID and store in DB for Event Subscription API to reduce key size.
* Connector Client plugins have been released for V1 and V2.

### Known Issue
* Event unsubscribe API response message for DEVICE_DELETION eventID need to be changed.
  
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
