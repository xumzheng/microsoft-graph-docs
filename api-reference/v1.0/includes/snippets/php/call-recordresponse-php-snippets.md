---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new RecordResponsePostRequestBody();


$requestRequestBody->setBargeInAllowed(True);
$requestRequestBody->setClientContext('d45324c1-fcb5-430a-902c-f20af696537c');
$promptsArray = [];

$prompts1 = new Prompt();

$prompts1AdditionalData = [
		"@odata.type" => '#microsoft.graph.mediaPrompt',
	];
$prompts1->setAdditionalData($prompts1AdditionalData);

$promptsArray []= $prompts1;
$requestRequestBody->setPrompts($promptsArray);
$requestRequestBody->setMaxRecordDurationInSeconds(10);
$requestRequestBody->setInitialSilenceTimeoutInSeconds(5);
$requestRequestBody->setMaxSilenceTimeoutInSeconds(2);
$requestRequestBody->setPlayBeep(True);
$requestRequestBody->setStopTones( [
'#','1','*',],
$result =  $graphClient->communications()->callsById('call-id')->recordResponse()->post($requestRequestBody);


```