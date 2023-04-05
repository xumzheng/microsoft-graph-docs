---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = NamedLocation()
request_body.set@odatatype('#microsoft.graph.countryNamedLocation')

request_body.setDisplayName('Updated named location without unknown countries and regions')

additionalData = [
'countriesAndRegions' => ['CA', 'IN', ],
'includeUnknownCountriesAndRegions' => false,
];
request_body.setAdditionalData(additionalData)




result = await client.identity_conditionalAccess_namedLocationsby_id('namedLocation-id').patch(request_body)


```