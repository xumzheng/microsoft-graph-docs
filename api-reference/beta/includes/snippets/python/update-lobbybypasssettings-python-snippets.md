---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = OnlineMeeting();
lobbyBypassSettings = LobbyBypassSettings();
lobbyBypassSettings.setIsDialInBypassEnabled(true);


requestBody.setLobbyBypassSettings($lobbyBypassSettings);


result = await client.me().onlineMeetingsById('onlineMeeting-id').patch(requestBody);


```