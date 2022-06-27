---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new SchedulePutRequestBody();


$requestRequestBodyAdditionalData = [
	"enabled" => True,
	"timeZone" => 'America/Chicago',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->teamsById('team-id')->schedule()->put($requestRequestBody);


```