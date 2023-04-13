---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = OnlineMeeting()
lobbyBypassSettings = LobbyBypassSettings()
lobbyBypassSettings.isDialInBypassEnabled = true


request_body.lobbyBypassSettings = lobbyBypassSettings



result = await client.me.onlineMeetings_by_id('onlineMeeting-id').patch(request_body = request_body)


```