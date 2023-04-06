---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = NamedLocation()
request_body.set@odatatype('#microsoft.graph.countryNamedLocation')

request_body.setDisplayName('Named location with unknown countries and regions')

additionalData = [
'countriesAndRegions' => ['US', 'GB', ],
'includeUnknownCountriesAndRegions' => true,
];
request_body.setAdditionalData(additionalData)



request_config = NamedLocationsRequestBuilderPostRequestConfiguration(
request_config = NamedLocationsRequestBuilderPostRequestConfiguration(query_params=)


result = await client.identity.conditionalAccess.namedLocations.post(request_body, headers=)


```