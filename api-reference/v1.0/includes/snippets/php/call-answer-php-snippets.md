---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new AnswerPostRequestBody();


$requestRequestBody->setCallbackUri('callbackUri-value');

$mediaConfig = new MediaConfig();
$requestRequestBody->setMediaConfig($mediaConfig);


$mediaConfigAdditionalData = [
	"@odata.type" => '#microsoft.graph.appHostedMediaConfig',
	"blob" => '<Media Session Configuration Blob>',
];
$mediaConfig->setAdditionalData($mediaConfigAdditionalData);

$acceptedModalitiesArray = [];
'audio',$acceptedModalitiesArray []= $acceptedModalities1;
$requestRequestBody->setAcceptedModalities($acceptedModalitiesArray);
$requestRequestBody->setParticipantCapacity(200);
$result =  $graphClient->communications()->callsById('call-id')->answer()->post($requestRequestBody);


```