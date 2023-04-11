---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AdministrativeUnit()
request_body.displayName = 'Seattle District Technical Schools'

request_body.description = 'Seattle district technical schools administration'

request_body.visibility = 'HiddenMembership'



request_configuration = AdministrativeUnitsRequestBuilderPostRequestConfiguration(
)


result = await client.directory.administrativeUnits.post(request_body = request_body)


```