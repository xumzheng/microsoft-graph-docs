---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = UserAttributeAssignmentsRequestBuilderGetRequestConfiguration(
request_config = UserAttributeAssignmentsRequestBuilderGetRequestConfiguration(query_params=query_params = UserAttributeAssignmentsRequestBuilderGetQueryParameters()
query_params.expand = ["userAttribute"]

)
query_params = UserAttributeAssignmentsRequestBuilderGetQueryParameters()
query_params.expand = ["userAttribute"]

)


result = await client.identity.b2xUserFlows_by_id('b2xIdentityUserFlow-id').userAttributeAssignments.get(request_config, headers=request_config)


```