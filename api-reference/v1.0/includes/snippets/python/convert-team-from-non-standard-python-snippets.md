---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = Team();
requestBody.setDisplayName('My Class Team');

requestBody.setDescription('My Class Team’s Description');

additionalData = [
'template@odata.bind' => 'https://graph.microsoft.com/v1.0/teamsTemplates(\'educationClass\')', 
];
requestBody.setAdditionalData(additionalData);




result = await client.teams().post(requestBody);


```