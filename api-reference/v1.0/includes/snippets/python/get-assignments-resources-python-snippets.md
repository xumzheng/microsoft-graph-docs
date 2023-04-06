---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = AssignmentsRequestBuilderGetRequestConfiguration(
request_configuration = AssignmentsRequestBuilderGetRequestConfiguration(query_params=query_params = AssignmentsRequestBuilderGetQueryParameters()
query_params['expand'] = ["resources"]

)
query_params = AssignmentsRequestBuilderGetQueryParameters()
query_params['expand'] = ["resources"]

)


result = await client.education.classes_by_id('educationClass-id').assignments.get(request_configuration)


```