## mID Connector v2.5.0

<br/>

**Date** 2022-09-29

### **Docker Download**

### kobil/kobil-cloud-connector:2.5.0
**DIGEST:** sha256:e32d446e156fc5a991643870460bbf46fd0dce14822878f7a074a389f4283bbe
### kobil/kobil-cloud-pooler:3.0.2
**DIGEST:** sha256:3ea37cc02de764c061e41726ec1713cd0a770d368a3fc4ac1cd1649f19d041b7

<br/>

### **Azurecr Download**
- **Connector:** kobilsystems.azurecr.io/idp/ssms-connector:2.5.0  
- **Pooler:** kobilsystems.azurecr.io/idp/ssms-pooler:3.0.2
<br/>

-----------------------------------
 
### Changed 
* Accommodating pooler related queuing changes and kobil core jar changes


## Kobil Core Version: 3.0.0-dev.39

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
