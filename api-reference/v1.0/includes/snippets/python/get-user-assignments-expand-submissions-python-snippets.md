---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

query_params = AssignmentsRequestBuilder.AssignmentsRequestBuilderGetQueryParameters(
		expand = ["submissions"],
)

request_configuration = AssignmentsRequestBuilderGetRequestConfiguration(
query_parameters = query_params,
)


result = await client.education.users_by_id('educationUser-id').assignments.get(request_configuration = request_configuration)


```