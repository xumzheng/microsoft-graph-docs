---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = ExportPersonalDataPostRequestBody();
requestBody.setStorageLocation('storageLocation-value');



await client.usersById('user-id').exportPersonalData().post(requestBody);


```