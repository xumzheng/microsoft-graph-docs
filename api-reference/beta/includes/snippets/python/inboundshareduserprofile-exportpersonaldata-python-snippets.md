---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = ExportPersonalDataPostRequestBody();
requestBody.setStorageLocation('MyStorageAccount');



awaitclient.directory().inboundSharedUserProfilesById('inboundSharedUserProfile-userId').exportPersonalData().post(requestBody);


```