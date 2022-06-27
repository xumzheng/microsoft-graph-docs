---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new OnlineMeeting();



$lobbyBypassSettings = new LobbyBypassSettings();
$requestRequestBody->setLobbyBypassSettings($lobbyBypassSettings);


$lobbyBypassSettings->setIsDialInBypassEnabled(True);

$result =  $graphClient->me()->onlineMeetingsById('onlineMeeting-id')->patch($requestRequestBody);


```