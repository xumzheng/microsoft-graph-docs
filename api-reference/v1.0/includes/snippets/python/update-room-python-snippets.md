---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = Place();
request_body.set@odatatype('microsoft.graph.room');

additionalData = [
'nickname' => 'Conf Room', 
'building' => '1', 
'label' => '100', 
'capacity' => 50,
'isWheelChairAccessible' => false,
];
request_body.setAdditionalData(additionalData);




result = await client.placesById('place-id').patch(request_body);


```