## Kobil Cloud Connector v1.4.1

<br/>

### **Docker Download**

### kobil/kobil-cloud-connector:1.4.1
**DIGEST:** sha256:079c473d80a1951a537ca69f786ce0eaaf588e4a7c4cf0a5afea7e3541eaf777

<br/>

### kobil/kobil-cloud-pooler:1.4.1
**DIGEST:** sha256:9d7612d3ee1fcb83952f079511e164aa4c75bda094f1a92da211459c6862c0ed

------------------------------------
<br/>

### Bug Fix
* Fixed: Validation of of ssl certificates for callback url supported API’s

<br/>

### Known issues
* Semantic errors with downloaded swagger json.

<br/>

### Not Supported
* AWS ElasticCache does not work with redis.
* Redis sentinal is not supported.

<br/>

### SSMS Version
* 2.9.x supported
* 3.1.x not supported

<br/>

### Tested Server
* MultiTenant: 2.9.0.68478
* SingleTenant: 2.8.9.67994

<br/>

### Dependencies
* **Docker Engine 19.03.8**
https://docs.docker.com/engine/release-notes/#19038
* **Docker Compose 1.25.5**
https://github.com/docker/compose/releases

