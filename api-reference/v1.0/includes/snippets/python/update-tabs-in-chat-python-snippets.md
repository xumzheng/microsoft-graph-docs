---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = TeamsTab()
request_body.setDisplayName('My Contoso Tab - updated again')



result = await client.chatsById('chat-id').tabsById('teamsTab-id').patch(request_body)


```