---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new Participant-idPostRequestBody();


$requestRequestBodyAdditionalData = [
	"clientContext" => 'd45324c1-fcb5-430a-902c-f20af696537c',
	"participantMixerLevels" =>  [
	],
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->communications()->callsById('call-id')->participantsById('participant-id')->post($requestRequestBody);


```