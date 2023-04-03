---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = Team();
requestBody.setDisplayName('My Sample Team');

requestBody.setDescription('My Sample Team’s Description');

additionalData = [
'template@odata.bind' => 'https://graph.microsoft.com/v1.0/teamsTemplates(\'standard\')', 
];
requestBody.setAdditionalData(additionalData);




requestResult = graphServiceClient.teams().post(requestBody);


```