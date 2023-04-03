---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = OnlineMeeting();
lobbyBypassSettings = LobbyBypassSettings();
lobbyBypassSettings.setIsDialInBypassEnabled(true);


requestBody.setLobbyBypassSettings($lobbyBypassSettings);


requestResult = graphServiceClient.me().onlineMeetingsById('onlineMeeting-id').patch(requestBody);


```