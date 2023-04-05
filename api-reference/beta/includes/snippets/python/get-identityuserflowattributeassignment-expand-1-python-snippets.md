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


result = await client.identity_b2cUserFlowsby_id('b2cIdentityUserFlow-id')_userAttributeAssignments.get(request_config)


```