---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ReferenceCreate()
request_body.@odataid = 'https://graph.microsoft.com/odata/groups(\'dc3d2ce5-7c5e-4dca-a0ef-2145bf6e53ef\')'



request_configuration = RefRequestBuilderPostRequestConfiguration(
)


await client.policies.mobileDeviceManagementPolicies_by_id('mobilityManagementPolicy-id').includedGroups.ref.post(request_body = request_body)


```