---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = NamedLocation();
requestBody.set@odatatype('#microsoft.graph.countryNamedLocation');

requestBody.setDisplayName('Updated named location without unknown countries and regions');

additionalData = [
'countriesAndRegions' => ['CA', 'IN', ],
'includeUnknownCountriesAndRegions' => false,
];
requestBody.setAdditionalData(additionalData);




result = await client.identity().conditionalAccess().namedLocationsById('namedLocation-id').patch(requestBody);


```