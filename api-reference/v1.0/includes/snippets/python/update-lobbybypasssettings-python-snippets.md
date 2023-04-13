---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = OnlineMeeting()
lobby_bypass_settings = LobbyBypassSettings()
lobbyBypassSettings.is_dial_in_bypass_enabled = True


request_body.lobby_bypass_settings = lobbyBypassSettings



result = await client.me.onlineMeetings_by_id('onlineMeeting-id').patch(request_body = request_body)


```