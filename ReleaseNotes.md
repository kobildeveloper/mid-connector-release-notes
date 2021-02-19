## mID Connector v2.0.4

<br/>

### **Docker Download**

### kobil/kobil-cloud-connector:2.0.4
**DIGEST:** sha256:a48845a090c9b2e56bed8b01322dcdef2f8b6bc989cb3e1acf3f3c6e7178334e

<br/>

### kobil/kobil-cloud-pooler:2.0.2
**DIGEST:** sha256:6723a2a830ceb22b920218364d35146bdc16cf129cbc806bee8a30c2d9d16d6f

------------------------------------
<br/>



<br/>

### What's new
* Added new request body parameter callBackHeaders in create transaction api, HashMap<String, String> to send header parameters for the given callback URL and this parameter is optional
 
 

### Bug Fix
* Fixed multiple callbacks for device activation cluster issue.

<br/>

<br/>

### Supported
* AWS ElasticCache supported for both clustered and standalone, without redis authentication

<br/>

### Not Supported
* Redis sentinal is not supported

<br/>

### SSMS Version
* 2.9.x supported
* 3.1.x supported


<br/>

### Tested Server
* MultiTenant: 2.9.0.68478, 3.1.2.71992
* SingleTenant: 2.8.9.67994

<br/>

### Dependencies
* **Docker Engine 19.03.8**
https://docs.docker.com/engine/release-notes/#19038
* **Docker Compose 1.25.5**
https://github.com/docker/compose/releases


