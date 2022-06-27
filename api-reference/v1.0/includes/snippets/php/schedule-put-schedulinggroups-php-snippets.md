---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new SchedulingGroup-idPutRequestBody();


$requestRequestBodyAdditionalData = [
	"displayName" => 'Cashiers',
	"isActive" => True,
	"userIds" => ['c5d0c76b-80c4-481c-be50-923cd8d680a1','2a4296b3-a28a-44ba-bc66-0274b9b95851',],
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$requestConfiguration = new SchedulingGroupRequestBuilderPutRequestConfiguration();

$headers = [
"Prefer" => "return=representation",
];

$requestConfiguration->headers = $headers;


$result =  $graphClient->teamsById('team-id')->schedule()->schedulingGroupsById('schedulingGroup-id')->put($requestRequestBody, $requestConfiguration);


```