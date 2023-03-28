---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new Extension();
$requestBody->set@odatatype('microsoft.graph.openTypeExtension');

$additionalData = [
'extensionName' => 'Com.Contoso.Deal', 
'companyName' => 'Alpine Skis', 
'dealValue' => 1010100,
'expirationDate' => '2015-07-03T13:04:00.000Z', 
];
$requestBody->setAdditionalData($additionalData);




$requestResult = $graphServiceClient->groupsById('group-id')->eventsById('event-id')->extensions()->post($requestBody);


```