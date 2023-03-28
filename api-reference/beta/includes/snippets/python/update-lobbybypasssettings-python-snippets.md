---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new OnlineMeeting();
$lobbyBypassSettings = new LobbyBypassSettings();
$lobbyBypassSettings.setIsDialInBypassEnabled(true);


$requestBody.setLobbyBypassSettings($lobbyBypassSettings);


$requestResult = $graphServiceClient.me().onlineMeetingsById('onlineMeeting-id').patch($requestBody);


```