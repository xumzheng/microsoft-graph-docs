---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = Team();
additionalData = [
'template@odata.bind' => 'https://graph.microsoft.com/v1.0/teamsTemplates(\'standard\')', 
'group@odata.bind' => 'https://graph.microsoft.com/v1.0/groups(\'71392b2f-1765-406e-86af-5907d9bdb2ab\')', 
];
requestBody.setAdditionalData(additionalData);




result = await client.teams().post(requestBody);


```