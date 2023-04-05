---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = UserAttributeAssignmentsRequestBuilderGetRequestConfiguration()

query_params = UserAttributeAssignmentsRequestBuilderGetQueryParameters()
query_params.expand = ["userAttribute"]

request_config.queryParameters = query_params


result = await client.identity.b2xUserFlows_by_id('b2xIdentityUserFlow-id').userAttributeAssignments.get(request_config)


```