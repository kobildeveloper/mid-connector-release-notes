## mID Connector v2.5.0

<br/>

**Date** 2022-11-02

### **Docker Download**

### kobil/kobil-cloud-connector:2.5.0
**DIGEST:** 
### kobil/kobil-cloud-pooler:2.5.0
**DIGEST:** 

<br/>

### **Azurecr Download**
- **Connector:** kobilsystems.azurecr.io/idp/ssms-connector:2.5.0  
- **Pooler:** kobilsystems.azurecr.io/idp/ssms-pooler:2.5.0
<br/>

------------------------------------
 
### Changed 
* Updated cloud connector service image version to 2.4.3 which uses the `kobilsystems.azurecr.io/it-solutions/base-images/micro/jre17:1.1.0`

* 

### Note: 

## Kobil Core Version: 2.2.1 

### Support Versions
Connector Client plugins: 2.4.2_v1, 2.4.2_v2 
 
### SSMS Version 
* 2.x.x supported 
* 3.x.x supported 

### Tested Server 
* MultiTenant: 3.4.1.75470 and 3.5.2.79434 
* SingleTenant: 2.8.11.76074 

### Note
* Before every deployment, Redis data should be cleared and restarted. 
