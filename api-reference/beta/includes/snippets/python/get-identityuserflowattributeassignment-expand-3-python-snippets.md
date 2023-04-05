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


result = await client.identity.b2cUserFlowsby_id('b2cIdentityUserFlow-id').userAttributeAssignmentsby_id('identityUserFlowAttributeAssignment-id').get(request_config)


```