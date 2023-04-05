---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = SubmissionsRequestBuilderGetRequestConfiguration()

query_params = SubmissionsRequestBuilderGetQueryParameters()
query_params.expand = ["outcomes"]

request_config.queryParameters = query_params


result = await client.education.classesby_id('educationClass-id').assignmentsby_id('educationAssignment-id').submissions.get(request_config)


```