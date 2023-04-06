---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Channel()
request_body.setDisplayName('Architecture Discussion')

request_body.setDescription('This channel is where we debate all future architecture plans')

request_body.setMembershipType(ChannelMembershipType('standard'))



result = await client.teams_by_id('team-id').channels.post(request_body, headers=)


```