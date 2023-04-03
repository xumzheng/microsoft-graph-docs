---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = Place();
requestBody.set@odatatype('microsoft.graph.workspace');

additionalData = [
'nickname' => 'Conf Room', 
'building' => '1', 
'label' => '100', 
'capacity' => 50,
'isWheelChairAccessible' => false,
];
requestBody.setAdditionalData(additionalData);




result = awaitclient.placesById('place-id').patch(requestBody);


```