## mID Connector v2.1.0

<br/>

### **Docker Download**

### kobil/kobil-cloud-connector:2.1.0
**DIGEST:** sha256:bec0ccaa7625b8751389807edc43ca114da36d2b5a90733ded778f60ad051c38

<br/>

### kobil/kobil-cloud-pooler:2.1.0
**DIGEST:** sha256:3e2c69aded575e458cef3fbec92dd65750f9b14685afb4282e6d1324d28c3706

------------------------------------
<br/>



<br/>

### Added
* ASM Management: GetUserDevice - userID retrieval in the response (Note - this will not be supported for the SSMS version which are less than 3.x.x)
 
 

### Changed
* ASM Service: PropertyType should support any one of the enum types (BYTE_ARRAY, INTEGER, STRING, BOOLEAN and DATE) and retreives the same with GetProperty response

<br/>

<br/>

### Supported
* AWS ElasticCache supported for both clustered and standalone, without redis authentication

<br/>

### Not Supported
* Redis sentinal is not supported

<br/>

### SSMS Version
* 2.x.x supported
* 3.x.x supported


<br/>

### Tested Server
* MultiTenant: 2.9.0.68478, 3.1.2.71992 and 3.4.1.75470
* SingleTenant: 2.8.11.76074

<br/>

### Dependencies
* **Docker Engine 19.03.8**
https://docs.docker.com/engine/release-notes/#19038
* **Docker Compose 1.25.5**
https://github.com/docker/compose/releases


