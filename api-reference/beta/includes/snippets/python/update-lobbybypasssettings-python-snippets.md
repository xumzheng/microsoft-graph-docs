---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = OnlineMeeting()
lobbyBypassSettings = LobbyBypassSettings()
lobbyBypassSettings.setIsDialInBypassEnabled(true)


request_body.setLobbyBypassSettings($lobbyBypassSettings)


result = await client.me.onlineMeetingsby_id('onlineMeeting-id').patch(request_body)


```