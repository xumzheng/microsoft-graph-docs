---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new TimeOffReason();
$additionalData = [
'displayName' => 'Vacation', 
'iconType' => 'plane', 
'isActive' => true,
];
$requestBody->setAdditionalData($additionalData);



$requestConfiguration = new TimeOffReasonRequestBuilderPutRequestConfiguration();

$headers = [
	'Prefer' => 'return=representation',
];

$requestConfiguration->headers = $headers;


$graphServiceClient->teamsById('team-id')->schedule()->timeOffReasonsById('timeOffReason-id')->put($requestBody, $requestConfiguration);


```