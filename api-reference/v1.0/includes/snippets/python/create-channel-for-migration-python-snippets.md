---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Channel()
request_body.displayName = 'Import_150958_99z'

request_body.description = 'Import_150958_99z'

request_body.createdDateTime = DateTime('2020-03-14T11:22:17.067Z')

additionalData = [
'@microsoft.graph.channelCreationMode' => 'migration', 
];
request_body.additionaldata(additionalData)





result = await client.teams_by_id('team-id').channels.post(request_body = request_body)


```