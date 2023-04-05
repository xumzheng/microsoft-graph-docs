---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = AssignmentsRequestBuilderGetRequestConfiguration()

query_params = AssignmentsRequestBuilderGetQueryParameters()
query_params.expand = ["submissions"]

request_config.queryParameters = query_params


result = await client.education_usersby_id('educationUser-id')_assignments.get(request_config)


```