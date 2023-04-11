---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

query_params = AppliesToRequestBuilder.AppliesToRequestBuilderGetQueryParameters(
				select = ["id","appId","displayName","createdDateTime"],
)

request_configuration = AppliesToRequestBuilderGetRequestConfiguration(
query_parameters = query_params,
)


result = await client.policies.appManagementPolicies_by_id('appManagementPolicy-id').appliesTo.get(request_configuration = request_configuration)


```