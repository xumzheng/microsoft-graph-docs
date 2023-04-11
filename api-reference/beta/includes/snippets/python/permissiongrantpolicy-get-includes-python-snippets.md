---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)


request_configuration = IncludesRequestBuilderGetRequestConfiguration(
)


result = await client.policies.permissionGrantPolicies_by_id('permissionGrantPolicy-id').includes.get()


```