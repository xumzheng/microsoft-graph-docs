---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = Team();
request_body.setDisplayName('My Sample Team');

request_body.setDescription('My Sample Team’s Description');

additionalData = [
'template@odata.bind' => 'https://graph.microsoft.com/v1.0/teamsTemplates(\'standard\')', 
];
request_body.setAdditionalData(additionalData);




result = await client.teams().post(request_body);


```