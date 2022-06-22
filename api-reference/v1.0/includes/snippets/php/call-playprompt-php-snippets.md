---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new PlayPromptPostRequestBody();


$requestRequestBody->setClientContext('d45324c1-fcb5-430a-902c-f20af696537c');
$promptsArray = [];

$prompts1 = new Prompt();

$prompts1AdditionalData = [
		"@odata.type" => '#microsoft.graph.mediaPrompt',
	];
$prompts1->setAdditionalData($prompts1AdditionalData);

$promptsArray []= $prompts1;
$requestRequestBody->setPrompts($promptsArray);
$result =  $graphClient->communications()->callsById('call-id')->playPrompt()->post($requestRequestBody);


```