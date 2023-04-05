---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = IdentityUserFlowAttributeAssignmentRequestBuilderGetRequestConfiguration()

query_params = IdentityUserFlowAttributeAssignmentRequestBuilderGetQueryParameters()
query_params.expand = ["userAttribute"]

request_config.queryParameters = query_params


result = await client.identity.b2cUserFlows._by_id('b2cIdentityUserFlow-id').userAttributeAssignments._by_id('identityUserFlowAttributeAssignment-id').get(request_config)


```