## mID Connector v2.4.1

<br/>

**Date** 2022-04-06

### **Docker Download**

### kobil/kobil-cloud-connector:2.4.1
**DIGEST:**  
### kobil/kobil-cloud-pooler:2.4.1
**DIGEST:** 

<br/>

### **Azurecr Download**
- **Connector:** kobilsystems.azurecr.io/idp/ssms-connector:2.4.1  
- **Pooler:** kobilsystems.azurecr.io/idp/ssms-pooler:2.4.1
<br/>

------------------------------------
 
### Changed 
* Upgraded version of  
   - Spring boot version: Old - 2.6.3; Current - 2.6.6 
   - jackson-databind: Old - 2.12.5; Current - 2.13.2.1  

### Kobil Core Version 2.2.0 

### Support Versions
Connector Client plugins: 2.4.0_v1, 2.4.0_v2 
 
### SSMS Version 
2.x.x supported 
3.x.x supported 

### Tested Server 
* MultiTenant: 3.4.1.75470 , 3.5.2.79434 and 3.6.1.81437 
* SingleTenant: 2.8.11.76074 

### Note
* The vulnerabilities are fixed for all the dependencies of Connector. However, there are vulnerabilities in the base image of java that will be addressed in future releases. 
* Before every deployment, Redis data should be cleared and restarted. 
