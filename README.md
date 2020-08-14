
## mID Connector v2.0.1

<br/>

### **Docker Download**

### kobil/kobil-cloud-connector:2.0.1
**DIGEST:** sha256:d17ae5e187a6ffe96f3b19a6fb46c1eb0191eb9077c6cd3047de214f96b22a17

<br/>

### kobil/kobil-cloud-pooler:2.0.0
**DIGEST:** sha256:580f217dc5fc860050756d3c54ade34ef4f9418082f5d32e7187ba142944b24d

------------------------------------
<br/>

### What's new
* New parameter appName has been added in CreateTransaction API, to restrict transactions to devices registered using particular app names


<br/>

### Known issues
* Semantic errors with downloaded swagger json

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

