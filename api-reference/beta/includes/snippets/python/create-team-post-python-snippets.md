---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = Team();
requestBody.setDisplayName('My Sample Team');

requestBody.setDescription('My Sample Team’s Description');

additionalData = [
'template@odata.bind' => 'https://graph.microsoft.com/beta/teamsTemplates(\'standard\')', 
];
requestBody.setAdditionalData(additionalData);




result = await client.teams().post(requestBody);


```