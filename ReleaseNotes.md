## mID Connector v4.1.0-rc.1

<br/>

**Date** 2022-11-25

### **Docker Download**
### kobil/kobil-cloud-connector:4.1.0-rc.1
**DIGEST:** digest: sha256:dbdbc60f4ec57d9fc5c2929b623c2ab0d362aa184ae70435b52e16ba2d3a8104

<br/>

### **Azurecr Download**
- **Connector:** kobilsystems.azurecr.io/idp/ssms-connector:4.1.0-rc.1
<br/>
 
### Added 
* Added support to retrieve transaction, QR result from redis. 
* Introduced pollfromredis queryparam in transaction and qr API's to take result from redis
* Updated kobil core version to 4.0.1
* Added request param pollfromredis for the  following API’s 
    - StartTransaction
    - GetTransactionResult
    - CreateOnlineQR
    - VerifyOnlineQR
    - AddNewDeviceTransaction

## Kobil Core Version: 4.0.1

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
