---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = NamedLocation()
request_body.@odatatype = '#microsoft.graph.countryNamedLocation'

request_body.displayName = 'Named location with unknown countries and regions'

additionalData = [
'countriesAndRegions' => ['US', 'GB', ],
'includeUnknownCountriesAndRegions' => true,
];
request_body.additionaldata(additionalData)




request_configuration = NamedLocationsRequestBuilderPostRequestConfiguration(
)


result = await client.identity.conditionalAccess.namedLocations.post(request_body = request_body)


```