## mID Connector v2.0.0-beta.204

<br/>

### **Docker Download**


### kobil/kobil-cloud-connector:2.0.0-beta.204
**DIGEST:** sha256:6f37f2319c6dc2786e72536fa2e4c772237203d06ee10cf946cb8c73ba3eef68

<br/>

### kobil/kobil-cloud-pooler:2.0.0-beta.48
**DIGEST:** sha256:e6366e8c51bcbbc27fe445cee4908c5c7f746add0c840eb57aa29f1769ea0bd6

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


<br/>

### Isolated changes
* Fixed: Changed the response code for LockUser, UnLockUser, LockDevice and UnlockDevice API’s conflict case in Asm Management Controller.
* Fixed: Changed the response code for the `Functionality unsupported for Multi-tenant’ scenario in RenameUser API.


<br/>

### Configuration  Changes 
* Improvised to handle proper functionality even when truststore is disabled in connector.properties.

<br/>

### Bug Fixes
* Restricted sensitive data leakage in generateAuthKey on mID Connector UI Extension.
* Fix applied to enable user registration with dev2 credentials via mID Connector UI Extension, when GetTenants and CreateTenant API's do not function.
* Fixed error while retrieving Activation code with qr format as "MPOWER" during retrieval and secret=true during Activation code creation.


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


### Not Included in Package (Until final release)
Documentation of connector.aws1.kobil.com is not included in this release. Currently documentation is in-progress stage, which will be included in our final release.
