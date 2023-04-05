---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = EducationSubmissionRequestBuilderGetRequestConfiguration()

query_params = EducationSubmissionRequestBuilderGetQueryParameters()
query_params.expand = ["*"]

request_config.queryParameters = query_params


result = await client.education_classesby_id('educationClass-id')_assignmentsby_id('educationAssignment-id')_submissionsby_id('educationSubmission-id').get(request_config)


```