---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = ReferenceCreate();
requestBody.set@odataid('https://graph.microsoft.com/beta/directoryObjects/{id}');



graphServiceClient.devicesById('device-id').registeredUsers().ref().post(requestBody);


```