---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

query_params = UserAttributeAssignmentsRequestBuilder.UserAttributeAssignmentsRequestBuilderGetQueryParameters(
				expand = ["userAttribute"],
)

request_configuration = UserAttributeAssignmentsRequestBuilderGetRequestConfiguration(
query_parameters = query_params,
)


result = await client.identity.b2xUserFlows_by_id('b2xIdentityUserFlow-id').userAttributeAssignments.get(request_configuration = request_configuration)


```