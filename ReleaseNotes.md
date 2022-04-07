## mID Connector v2.4.1

<br/>

**Date** 2022-04-07

### **Docker Download**

### kobil/kobil-cloud-connector:2.4.1
**DIGEST:** sha256:0f932d853ce7715f898d72dcc29b550fd5c3537d0dba857d4d6d5727412d5931 
### kobil/kobil-cloud-pooler:2.4.1
**DIGEST:** sha256:73d25ac006c1ae07bee2744d1a45d15be07c276732a39d47ba25119fd49dd867

<br/>

### **Azurecr Download**
- **Connector:** kobilsystems.azurecr.io/idp/ssms-connector:2.4.1  
- **Pooler:** kobilsystems.azurecr.io/idp/ssms-pooler:2.4.1
<br/>

------------------------------------
 
### Changed 
* Dependencies updated in mIDConnector: 
  - Spring boot version: Old - 2.6.3; Current - 2.6.6 
  - jackson-databind: Old - 2.12.5; Current - 2.13.2.1 
* Dependencies updated in KOBIL UI Extension: 
  - Spring boot version: Old - 2.6.3; Current - 2.6.6 

## Kobil Core Version: 2.2.0 

### Support Versions
Connector Client plugins: 2.4.1_v1, 2.4.1_v2 
 
### SSMS Version 
* 2.x.x supported 
* 3.x.x supported 

### Tested Server 
* MultiTenant: 3.4.1.75470 , 3.5.2.79434 and 3.6.1.81437 
* SingleTenant: 2.8.11.76074 

### Note
* The vulnerabilities are fixed for all the dependencies of Connector. However, there are vulnerabilities in the base image of java that will be addressed in future releases. 
* Before every deployment, Redis data should be cleared and restarted. 
