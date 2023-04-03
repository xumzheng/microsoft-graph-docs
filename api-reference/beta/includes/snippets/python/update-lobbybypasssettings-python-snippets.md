---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = OnlineMeeting();
lobbyBypassSettings = LobbyBypassSettings();
lobbyBypassSettings.setIsDialInBypassEnabled(true);


requestBody.setLobbyBypassSettings($lobbyBypassSettings);


result = awaitclient.me().onlineMeetingsById('onlineMeeting-id').patch(requestBody);


```