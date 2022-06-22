---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new TimeCard-idPutRequestBody();


$requestRequestBodyAdditionalData = [
	"userId" => '70e47528-2fae-42b5-9d8e-ee73ccd90603',
	"state" => 'clockedOut',
	"confirmedBy" => 'None',
	"notes" => null,
	"breaks" =>  [
	],
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->teamsById('team-id')->schedule()->timeCardsById('timeCard-id')->put($requestRequestBody);


```