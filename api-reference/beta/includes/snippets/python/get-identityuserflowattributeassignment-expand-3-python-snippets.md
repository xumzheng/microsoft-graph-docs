---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = IdentityUserFlowAttributeAssignmentRequestBuilderGetRequestConfiguration(
query_params = IdentityUserFlowAttributeAssignmentRequestBuilderGetQueryParameters()
query_params.expand = ["userAttribute"]

)


result = await client.identity.b2cUserFlows_by_id('b2cIdentityUserFlow-id').userAttributeAssignments_by_id('identityUserFlowAttributeAssignment-id').get(request_config)


```