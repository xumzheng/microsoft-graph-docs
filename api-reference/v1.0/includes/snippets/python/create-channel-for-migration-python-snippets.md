---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = Channel();
requestBody.setDisplayName('Import_150958_99z');

requestBody.setDescription('Import_150958_99z');

requestBody.setCreatedDateTime(DateTime('2020-03-14T11:22:17.067Z'));

additionalData = [
'@microsoft.graph.channelCreationMode' => 'migration', 
];
requestBody.setAdditionalData(additionalData);




result = awaitclient.teamsById('team-id').channels().post(requestBody);


```