## mID Connector v2.7.0

<br/>

**Date** 2022-11-04

### **Docker Download**

### kobil/kobil-cloud-connector:2.7.0
**DIGEST:** sha256:8729223e9a0a18b76684d393acdc348d1f08e25a6356b5b952c4b6f5929ec49b

<br/>

### **Azurecr Download**
- **Connector:** kobilsystems.azurecr.io/idp/ssms-connector:2.7.0  
<br/>

------------------------------------
 
### Changed 
* ci lib version to 13.10.0
* gitlab.kobil.com:4567/development/devops/base-images/jre17-micro base image to 1.3.0

### Added 
* labels to dockerfile


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
