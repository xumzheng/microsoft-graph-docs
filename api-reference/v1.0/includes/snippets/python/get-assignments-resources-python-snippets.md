---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = AssignmentsRequestBuilderGetRequestConfiguration()

query_params = AssignmentsRequestBuilderGetQueryParameters()
query_params.expand = ["resources"]

request_config.queryParameters = query_params


result = await client.education_classesby_id('educationClass-id')_assignments.get(request_config)


```