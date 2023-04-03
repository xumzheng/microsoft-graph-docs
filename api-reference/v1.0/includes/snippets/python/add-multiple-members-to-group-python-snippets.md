---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = Group();
additionalData = [
'members@odata.bind' => ['https://graph.microsoft.com/v1.0/directoryObjects/{id}', 'https://graph.microsoft.com/v1.0/directoryObjects/{id}', 'https://graph.microsoft.com/v1.0/directoryObjects/{id}', ],
];
requestBody.setAdditionalData(additionalData);




result = awaitclient.groupsById('group-id').patch(requestBody);


```