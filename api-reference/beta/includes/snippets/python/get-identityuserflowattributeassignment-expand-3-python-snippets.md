---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

query_params = IdentityUserFlowAttributeAssignmentRequestBuilder.IdentityUserFlowAttributeAssignmentRequestBuilderGetQueryParameters(
				expand = ["userAttribute"],
)

request_configuration = IdentityUserFlowAttributeAssignmentRequestBuilderGetRequestConfiguration(
query_parameters = query_params,
)


result = await client.identity.b2cUserFlows_by_id('b2cIdentityUserFlow-id').userAttributeAssignments_by_id('identityUserFlowAttributeAssignment-id').get(request_configuration = request_configuration)


```