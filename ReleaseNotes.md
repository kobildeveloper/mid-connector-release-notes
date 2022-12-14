## mID Connector v4.1.0

<br/>

**Date** 2022-12-13

### **Docker Download**
### kobil/kobil-cloud-connector:4.1.0
**DIGEST:** digest: sha256:67835bf234d9da511412b277ee0151df15ee184b7a08c85f71e1d0dc245ec994 

<br/>

### **Azurecr Download**
- **Connector:** kobilsystems.azurecr.io/idp/ssms-connector:4.1.0
<br/>
 
### Added 
* Sonarqube scan job.
* Support to expose prometheus metrics.
* Ping endpoint to provide liveliness probe.
* Added support to retrieve transaction, QR result from redis, based on the Environment Variable configuration HANDLE_DEVICE_EVENTS_WITH_REDIS by default the value is configured to false.
* Added request param pollfromredis for the  following API’s to take result from redis
    - StartTransaction
    - GetTransactionResult
    - CreateOnlineQR
    - VerifyOnlineQR
    - AddNewDeviceTransaction
* Added support to enable connection pooling on opening a socket connection with SSMS. By default it is disabled which could be enable by setting env variable DISABLE_HTTP_DISCONNECTION to true.
* Support to expose prometheus metrics.

## Changed
* Provided backward compatibility for connector version 2.6.0
* Updated responses of continuous polling scenario in QR and transaction endpoint based on HANDLE_DEVICE_EVENTS_WITH_REDIS env variable
* Changed tomcat version to 9.0.68
* Updated kobilcore version to 4.0.1
* CI Lib 14.6.2
 

## Kobil Core Version: 4.0.1

### Support Versions
Connector Client plugins: 4.1.0_v1, 4.1.0_v2 
 
### SSMS Version 
* 2.x.x supported 
* 3.x.x supported

### Tested Server 
* MultiTenant: 3.4.1.75470 and 3.5.2.79434 
* SingleTenant: 2.8.11.76074 

### Note
* Before every deployment, Redis data should be cleared and restarted. 
