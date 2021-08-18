
## mID Connector v2.0.0

<br/>

### **Docker Download**

### kobil/kobil-cloud-connector:2.0.0
**DIGEST:** sha256:d57c87b6cbc7ca85003354b2c4451705c118159135aed0940bd160c12e9669f0

<br/>

### kobil/kobil-cloud-pooler:2.0.0
**DIGEST:** sha256:580f217dc5fc860050756d3c54ade34ef4f9418082f5d32e7187ba142944b24d

------------------------------------
<br/>

### What's new
* Added support for 3.1.x SSMS server.
  * "mID connector V1” supports the 2.9.x  version of SSMS 
  * "mID connector V2” supports the 3.1.x version of SSMS
* Added PamLockUser REST API to lock Pam users.
* Added PamUnLockUser REST API to Unlock Pam users.
* Branding changed from “KOBIL Cloud Connector” to “mID Connector”.
* Updated KOBIL logo.
* Refactored the module name based on the business context.


<br/>

### Improvements
* Refined message content in the response for invalid TimeStamp (which does not impact the overall functionality) in these APIs - SetDeviceProperty, GetDeviceProperties, DeleteDeviceProperty, SetUserProperty, GetUserProperties, DeleteUserProperty, CreateGroupProperty, GetGroupProperties, DeleteGroupProperty.
* Restricted future date for GetManagementCredentials, GetAuditingItems and GetMonitoring.
* Added support for alphanumeric characters and special characters for “password” parameter in PamCreateUser.
* Improvised “SetGlobalPin” to accommodate "ResetGlobalPin" functionality. When the 'pin' parameter is empty during the SetGlobalPin API call, an auto-generated pin is assigned to the user.
* Refactored the response code, status and message used in the connector for consistency.
* Updated the response status and message for mandatory parameters in API’s used in the connector.
* “deviceType” is by default set to null when softwareType is set to “APP” for Apps related API's in Asm Management Controller.
* Refined the response for transaction not found scenario in CancelTransaction API.
* “callbackurl” is made mandatory when pollforresult is set to false for CreateTransaction API.
* “createactivationcode” query parameter removed from request for PamCreateUser.
* Added poolerv1 and poolerv2 actuator health check.

<br/>

### Isolated changes
* Fixed: Changed the response code for LockUser, UnLockUser, LockDevice and UnlockDevice API’s conflict case in Asm Management Controller.
* Fixed: Changed the response code for the `Functionality unsupported for Multi-tenant’ scenario in RenameUser API.
* Refactor the AccessToken API URL from v1/system/token to authentication/token

<br/>

### Configuration  Changes 
* Improvised to handle proper functionality even when truststore is disabled in connector.properties.

<br/>

### Bug Fixes
* Restricted sensitive data leakage in generateAuthKey on mID Connector UI Extension.
* Fix applied to enable user registration with dev2 credentials via mID Connector UI Extension, when GetTenants and CreateTenant API's do not function.
* Fixed error while retrieving Activation code with qr format as "MPOWER" during retrieval and secret=true during Activation code creation.
* Validation of ssl certificates for callback url supported API’s.

<br/>


### Upgrade Changes
* Redis (kobil_cloud_redis) should either be cleaned up or reset in order to upgrade to 2.0.0.

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

