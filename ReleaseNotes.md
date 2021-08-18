
## mID Connector v2.0.2

<br/>

### **Docker Download**

### kobil/kobil-cloud-connector:2.0.2
**DIGEST:** sha256:08daa3404a4ed72bb79028cfdb4a1fc4166710c4f66bd0c54bcc97958a9b92fe

<br/>

### kobil/kobil-cloud-pooler:2.0.0
**DIGEST:** sha256:580f217dc5fc860050756d3c54ade34ef4f9418082f5d32e7187ba142944b24d

------------------------------------
<br/>

### Added
* DeactivateTenant API support for ssms 3.x.x (Existing DeleteTenant API in 2.x.x serves the same purpose)


<br/>


### Fixed
* RenameUser API support for multitenant ssms 2.x.x and 3.x.x

<br/>

### Known issues
* Semantic errors with downloaded swagger json


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

