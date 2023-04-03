---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = ExportPersonalDataPostRequestBody();
requestBody.setStorageLocation('MyStorageAccount');



graphServiceClient.directory().inboundSharedUserProfilesById('inboundSharedUserProfile-userId').exportPersonalData().post(requestBody);


```