---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = AppliesToRequestBuilderGetRequestConfiguration(
request_configuration = AppliesToRequestBuilderGetRequestConfiguration(query_params=query_params = AppliesToRequestBuilderGetQueryParameters()
query_params['select'] = ["id","appId","displayName","createdDateTime"]

)
query_params = AppliesToRequestBuilderGetQueryParameters()
query_params['select'] = ["id","appId","displayName","createdDateTime"]

)


result = await client.policies.appManagementPolicies_by_id('appManagementPolicy-id').appliesTo.get(request_configuration)


```