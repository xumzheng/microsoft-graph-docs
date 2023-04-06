---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Place()
request_body.set@odatatype('microsoft.graph.workspace')

additionalData = [
'nickname' => 'Conf Room', 
'building' => '1', 
'label' => '100', 
'capacity' => 50,
'isWheelChairAccessible' => false,
];
request_body.setAdditionalData(additionalData)



request_config = PlaceRequestBuilderPatchRequestConfiguration(
request_config = PlaceRequestBuilderPatchRequestConfiguration(query_params=)


result = await client.places_by_id('place-id').patch(request_body, headers=)


```