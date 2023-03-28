---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new SchedulingGroup();
$additionalData = [
'displayName' => 'Cashiers', 
'isActive' => true,
'userIds' => ['c5d0c76b-80c4-481c-be50-923cd8d680a1', '2a4296b3-a28a-44ba-bc66-0274b9b95851', ],
];
$requestBody->setAdditionalData($additionalData);



$requestConfiguration = new SchedulingGroupRequestBuilderPutRequestConfiguration();

$headers = [
'Prefer' => 'return=representation',
];

$requestConfiguration->headers = $headers;


$graphServiceClient->teamsById('team-id')->schedule()->schedulingGroupsById('schedulingGroup-id')->put($requestBody, $requestConfiguration);


```