---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new PlayPromptPostRequestBody();


$requestRequestBody->setClientContext('d45324c1-fcb5-430a-902c-f20af696537c');
$promptsArray = [];

$promptsprompts1 = new Prompt();

$promptsprompts1AdditionalData = [
	"@odata.type" => '#microsoft.graph.mediaPrompt',
];
$promptsprompts1->setAdditionalData($promptsprompts1AdditionalData);

$promptsArray []= $promptsprompts1;
$requestRequestBody->setPrompts($promptsArray);
$requestRequestBody->setLoop(False);
$result =  $graphClient->communications()->callsById('call-id')->playPrompt()->post($requestRequestBody);


```