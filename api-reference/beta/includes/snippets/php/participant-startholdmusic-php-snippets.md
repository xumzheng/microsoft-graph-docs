---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new StartHoldMusicPostRequestBody();



$customPrompt = new Prompt();
$requestRequestBody->setCustomPrompt($customPrompt);


$customPromptAdditionalData = [
	"@odata.type" => '#microsoft.graph.mediaPrompt',
];
$customPrompt->setAdditionalData($customPromptAdditionalData);

$requestRequestBody->setClientContext('d45324c1-fcb5-430a-902c-f20af696537c');
$result =  $graphClient->communications()->callsById('call-id')->participantsById('participant-id')->startHoldMusic()->post($requestRequestBody);


```