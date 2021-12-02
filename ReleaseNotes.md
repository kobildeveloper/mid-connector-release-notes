## mID Connector v2.3.2

<br/>

**Date** 2021-12-02

### **Docker Download**

### kobil/kobil-cloud-connector:2.3.2
**DIGEST:**  sha256:a26045a58dc6cc3e273fb255fcd46cbe4d96c57b6112cf687c639034cf7c00d3
### kobil/kobil-cloud-pooler:2.3.0
**DIGEST:** sha256:b91e0815a8962444a7275c2f85f9d3d166d192fc75e1d8e9087cc41ce41e68e0

<br/>

### **Azurecr Download**
**Connector:** kobilsystems.azurecr.io/idp/ssms-connector:2.3.2  
**Pooler:** kobilsystems.azurecr.io/idp/ssms-pooler:2.3.0
<br/>

------------------------------------
            
### Fixes
* The response message for Event Unsubscribe API has been updated to reflect the type of event unsubscribed. (Known issue in V2.3.1).
* The Cloud Connector Client plugin has been generated using OpenAPI Generator tool (V5.3.0) instead of Swagger Codegen to pull in latest dependencies for the client jar. The dependencies in the Connector Plugin that are updated to latest versions are mentioned below:

            * Swagger Annotations: Old - 1.5.17; Current - 1.6.2
            * Okhttp3: Old - 2.7.5; Current - 4.9.1
            * Logging interceptor: Old - 2.7.5; Current - 4.9.1
            * Gson: Old - 2.8.1; Current - 2.8.6
            * Gson Fire: Old - 1.8.0; Current - 1.8.5
  
<br/>
  
### Not Supported
* Redis sentinal is not supported
<br/>
  
### Kobil Core Version
* 2.1.1

### Support Versions:
Connector Client plugins: 2.3.2_v1, 2.3.2_v2 
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
