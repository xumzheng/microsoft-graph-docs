---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = TeamsTab()
request_body.setDisplayName('My Contoso Tab - updated again')



result = await client.chatsby_id('chat-id')_tabsby_id('teamsTab-id').patch(request_body)


```