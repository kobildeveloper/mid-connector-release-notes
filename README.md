## mID Connector v2.1.1


<br/>

### **Docker Download**


### kobil/kobil-cloud-connector:2.1.1
**DIGEST:** sha256:9eab52db081b1966780bf13c6027f05f5eb4c78163e4a5c105e75674ca70a2f5

<br/>

### kobil/kobil-cloud-pooler:2.1.1
**DIGEST:** sha256:bbec088104cb6e1df2cc68ff95ad5faa30ff182c37ecea255147998a2e0ee708

------------------------------------
<br/>


### Changed
* Logs: Print in a single line with thread ID
* Logs: Mask transaction ID in the request, response
* Deployment: Run docker as non root user

<br/>

### Not Supported
* Redis sentinal is not supported

<br/>

### Kobil Core Version
* 2.1.0

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
https://docs.docker.com/engine/release-notes/19.03/
* **Docker Compose 1.28.6**
https://github.com/docker/compose/releases/tag/1.28.6
