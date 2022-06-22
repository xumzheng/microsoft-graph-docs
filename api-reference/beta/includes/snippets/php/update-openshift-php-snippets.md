---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new OpenShift-idPutRequestBody();


$requestRequestBodyAdditionalData = [
	"schedulingGroupId" => 'TAG_228940ed-ff84-4e25-b129-1b395cf78be0',
	"draftOpenShift" => null,
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->teamsById('team-id')->schedule()->openShiftsById('openShift-id')->put($requestRequestBody);


```