---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = ReferenceCreate();
requestBody.set@odataid('https://graph.microsoft.com/beta/users/0f933635-5b77-4cf4-a577-f78a5eb090a2');



await client.directoryRolesById('directoryRole-id').members().ref().post(requestBody);


```