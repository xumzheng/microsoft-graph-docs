---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = NamedLocation();
requestBody.set@odatatype('#microsoft.graph.countryNamedLocation');

requestBody.setDisplayName('Named location with unknown countries and regions');

additionalData = [
'countriesAndRegions' => ['US', 'GB', ],
'includeUnknownCountriesAndRegions' => true,
];
requestBody.setAdditionalData(additionalData);




result = awaitclient.identity().conditionalAccess().namedLocations().post(requestBody);


```