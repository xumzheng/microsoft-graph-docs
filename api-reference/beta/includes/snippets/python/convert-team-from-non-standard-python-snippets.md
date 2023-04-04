---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = Team();
request_body.setDisplayName('My Class Team');

request_body.setDescription('My Class Team’s Description');

additionalData = [
'template@odata.bind' => 'https://graph.microsoft.com/beta/teamsTemplates(\'educationClass\')', 
];
request_body.setAdditionalData(additionalData);




result = await client.teams().post(request_body);


```