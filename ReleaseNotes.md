## mID Connector v4.0.0

<br/>

**Date** 2022-11-18

### **Docker Download**
### kobil/kobil-cloud-connector:4.0.0
**DIGEST:** sha256:59e067744505c8508c370082a22bb8967a003ef967c9dd2f33ff953814b62699
<br/>

### **Azurecr Download**
- **Connector:** kobilsystems.azurecr.io/idp/ssms-connector:4.0.0
<br/>
 
### Added 
* Added support to retrieve transaction, QR result from redis.
* Introduced pollfromredis queryparam in transaction and qr API's to take result from redis
* updated kobil core to 4.0.0

## Kobil Core Version: 4.0.0-rc.296100

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
