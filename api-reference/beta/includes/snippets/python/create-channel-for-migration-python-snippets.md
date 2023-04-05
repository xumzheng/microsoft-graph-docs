---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Channel()
request_body.setDisplayName('Import_150958_99z')

request_body.setDescription('Import_150958_99z')

request_body.setCreatedDateTime(DateTime('2020-03-14T11:22:17.067Z'))

additionalData = [
'@microsoft.graph.channelCreationMode' => 'migration', 
];
request_body.setAdditionalData(additionalData)




result = await client.teamsby_id('team-id')_channels.post(request_body)


```