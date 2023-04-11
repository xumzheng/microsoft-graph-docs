---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AdministrativeUnit()
request_body.displayName = 'Greater Seattle District Technical Schools'



request_configuration = AdministrativeUnitRequestBuilderPatchRequestConfiguration(
)


result = await client.directory.administrativeUnits_by_id('administrativeUnit-id').patch(request_body = request_body)


```