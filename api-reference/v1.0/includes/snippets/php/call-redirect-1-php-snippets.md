---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new RedirectPostRequestBody();


$targetsArray = [];

$targetstargets1 = new InvitationParticipantInfo();

$targetstargets1AdditionalData = [
	"@odata.type" => '#microsoft.graph.invitationParticipantInfo',
];
$targetstargets1->setAdditionalData($targetstargets1AdditionalData);

$targetsArray []= $targetstargets1;
$requestRequestBody->setTargets($targetsArray);
$requestRequestBody->setCallbackUri('https://bot.contoso.com/api/calls/24701998-1a73-4d42-8085-bf46ed0ae039');
$result =  $graphClient->communications()->callsById('call-id')->redirect()->post($requestRequestBody);


```