---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = NamedLocation()
request_body.@odatatype = '#microsoft.graph.countryNamedLocation'

request_body.displayName = 'Updated named location without unknown countries and regions'

additionalData = [
'countriesAndRegions' => ['CA', 'IN', ],
'includeUnknownCountriesAndRegions' => false,
];
request_body.additionaldata(additionalData)




request_configuration = NamedLocationRequestBuilderPatchRequestConfiguration(
)


result = await client.identity.conditionalAccess.namedLocations_by_id('namedLocation-id').patch(request_body = request_body)


```