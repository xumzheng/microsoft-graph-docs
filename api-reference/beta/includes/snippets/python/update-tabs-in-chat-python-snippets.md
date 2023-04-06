---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = TeamsTab()
request_body.setDisplayName('My Contoso Tab - updated again')



result = await client.chats_by_id('chat-id').tabs_by_id('teamsTab-id').patch(request_body)


```