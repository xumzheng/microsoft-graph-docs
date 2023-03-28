---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new Place();
$requestBody->set@odatatype('microsoft.graph.workspace');

$additionalData = [
'nickname' => 'Conf Room', 
'building' => '1', 
'label' => '100', 
'capacity' => 50,
'isWheelChairAccessible' => false,
];
$requestBody->setAdditionalData($additionalData);




$requestResult = $graphServiceClient->placesById('place-id')->patch($requestBody);


```