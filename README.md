## mID Connector v2.6.0

<br/>

**Date** 2022-11-03

### **Docker Download**

### kobil/kobil-cloud-connector:2.6.0
**DIGEST:** sha256:f45cd4420382f6f4977a9ad6d41d301ff18549dead833aa8b59f5cd3825f7c7b
### kobil/kobil-cloud-pooler: 3.1.0
**DIGEST:** sha256:8d77a416f5a6a353d35ea30670387a05a32ab196567f8a1e57433f139b980741

<br/>

### **Azurecr Download**
- **Connector:** kobilsystems.azurecr.io/idp/ssms-connector:2.6.0
- **Pooler:** kobilsystems.azurecr.io/idp/ssms-pooler: 3.1.0
<br/>

------------------------------------
 
### Fixed 
* Redis cluster failover retry with dns instead of IP.


## Kobil Core Version: 

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
