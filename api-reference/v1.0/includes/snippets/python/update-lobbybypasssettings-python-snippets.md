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

request_config = OnlineMeetingRequestBuilderPatchRequestConfiguration(
request_config = OnlineMeetingRequestBuilderPatchRequestConfiguration(query_params=)


result = await client.me.onlineMeetings_by_id('onlineMeeting-id').patch(request_body, headers=)


```