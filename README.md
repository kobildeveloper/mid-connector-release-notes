## Kobil Cloud Connector v1.4.0

<br/>

### **Docker Download**


### kobil/kobil-cloud-connector:1.4.0
**DIGEST:** sha256:be0eb174c00aac28abe53db7963ec48c86a3fe7df4a82cd2c49a0a75ef1ea9c2

<br/>

### kobil/kobil-cloud-pooler:1.4.0
**DIGEST:** sha256:3da6dd6c5a386a98af90e208fc07a5d8615a9bb21ab9d33aa220f48a9681b384

------------------------------------
<br/>

### What's new
* GetTransactionResult: Added new feature which would be helpful for users in retrieving the latest transaction result using unique transaction ID over a period of 24 hours. This is configurable with pooler.transaction.persistenttimeout in seconds under connector.properties file. if this value is not mentioned, default time of 24 hours shall be taken into account and  alternatively, pooler.transaction.persistenttimeout = -1 disables this feature.
* Event Controller: Monitoring the SSMS events made easier now with this new module which helps the users in retrieving the details of dead events, subscribe/unsubscribe the events.

<br/>

### Improvements
* Increased API efficiency in handling the failure events with DeadEvents API for the major functionalities (CreateTransaction, VerifyOnlineQr).
* Users have provision to subscribe to their required events. Another interesting feature is to stream the live events (Available only for New device activation)  and display it to the user.
* Improvised pollforresult to accommodate callback support - If pollforresult = 'true', the callbackurl is not considered, the result of the function is returned along with the API response. If pollforresult = 'false' and a valid callbackurl is provided, the result of the function is delivered to the callbackurl, not with the API response.
* Refined message content in the response for better readability (which does not impact the overall functionality) in these API’s - DeleteAppUpdate, EditAppVersion, AssignVersionUpdate, EditApp, CreateApp.
* Added "ttl" optional parameter in CreateActivationCode API, this  API have an “activationNotAfter” option, which is hard to calculate the timestamp, so adding ttl in timeunit as an option in request body to calculate the “activationNotAfter”. (If “activationNotAfter” is present, then “ttl” should not be taken into account).
* Added pooler callback support.
* Broadcasting expiry of events.
* Added new support for displaying both online and offline devices in GetUserDevices API.

<br/>

### Isolated changes
* Fixed: Changed the response code for User creation conflict case in CreateKernalUser API.
* Fixed: Changed the response code for Tenant activation conflict case in ActivateTenant API.
* Fixed: Changed the response code for CreateOnlineQr and Create OfflineQr API.

<br/>

### Configuration  Changes 
* Retry limit - Property will attempt to fetch the data based on the configured retry limit count.
* Retry interval - Property for polling based on the configured milliseconds count.
* Default retrylimit is 3 and interval is 1000ms
* Maximum allowed retrylimit is 5  and maximum allowed interval is 30000ms (if these values are not set in connector.properties)

<br/>

### Bug Fixes
* Fixed: Issue in SetPassword API in updating the password in SSMS.
* Fixed: Changed the Uid response parameter key to UserID  in API’s - GetUserLogs and GetDeviceLogs.

<br/>

### Deprecation
* Callback url parameter in CreateActivationCode API. (Alternatively, use EventController. At Present, NEW DEVICE is added and made available for the user. In future, other events can be added)

<br/>

### Known issues
* Semantic errors with downloaded swagger json

<br/>

### Not Supported
* AWS ElasticCache does not work with redis.
* Redis sentinal is not supported

<br/>

### SSMS Version
* 2.9.x supported
* 3.x not supported

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
