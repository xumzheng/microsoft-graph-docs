---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Team()
request_body.setDisplayName('My Sample Team')

request_body.setDescription('My Sample Team’s Description')

request_body.setCreatedDateTime(DateTime('2020-03-14T11:22:17.067Z'))

additionalData = [
'@microsoft.graph.teamCreationMode' => 'migration', 
'template@odata.bind' => 'https://graph.microsoft.com/beta/teamsTemplates(\'standard\')', 
];
request_body.setAdditionalData(additionalData)




result = await client.teams.post(request_body)


```