---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = SubmissionsRequestBuilderGetRequestConfiguration(
request_config = SubmissionsRequestBuilderGetRequestConfiguration(query_params=query_params = SubmissionsRequestBuilderGetQueryParameters()
query_params.expand = ["outcomes"]

)
query_params = SubmissionsRequestBuilderGetQueryParameters()
query_params.expand = ["outcomes"]

)


result = await client.education.classes_by_id('educationClass-id').assignments_by_id('educationAssignment-id').submissions.get(request_config, headers=request_config)


```