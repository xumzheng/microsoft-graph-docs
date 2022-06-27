---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new AnswerPostRequestBody();


$requestRequestBody->setCallbackUri('https://bot.contoso.com/api/calls');
$acceptedModalitiesArray = [];
'audio',$acceptedModalitiesArray []= $acceptedModalitiesacceptedModalities1;
$requestRequestBody->setAcceptedModalities($acceptedModalitiesArray);

$mediaConfig = new MediaConfig();
$requestRequestBody->setMediaConfig($mediaConfig);


$mediaConfigAdditionalData = [
"@odata.type" => '#microsoft.graph.serviceHostedMediaConfig',
"preFetchMedia" => [],
];
$mediaConfig->setAdditionalData($mediaConfigAdditionalData);

$result =  $graphClient->communications()->callsById('call-id')->answer()->post($requestRequestBody);


```