---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = Channel();
requestBody.setDisplayName('Architecture Discussion');

requestBody.setDescription('This channel is where we debate all future architecture plans');

requestBody.setMembershipType(ChannelMembershipType('standard'));



result = await client.teamsById('team-id').channels().post(requestBody);


```