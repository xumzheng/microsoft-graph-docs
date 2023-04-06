---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = UserAttributeAssignmentsRequestBuilderGetRequestConfiguration(
request_configuration = UserAttributeAssignmentsRequestBuilderGetRequestConfiguration(query_params=query_params = UserAttributeAssignmentsRequestBuilderGetQueryParameters()
query_params['expand'] = ["userAttribute"]

)
query_params = UserAttributeAssignmentsRequestBuilderGetQueryParameters()
query_params['expand'] = ["userAttribute"]

)


result = await client.identity.b2cUserFlows_by_id('b2cIdentityUserFlow-id').userAttributeAssignments.get(request_configuration)


```