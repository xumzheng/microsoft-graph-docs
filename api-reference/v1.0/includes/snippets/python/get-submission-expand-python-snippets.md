---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = EducationSubmissionRequestBuilderGetRequestConfiguration(
request_configuration = EducationSubmissionRequestBuilderGetRequestConfiguration(query_params=query_params = EducationSubmissionRequestBuilderGetQueryParameters()
query_params['expand'] = ["*"]

)
query_params = EducationSubmissionRequestBuilderGetQueryParameters()
query_params['expand'] = ["*"]

)


result = await client.education.classes_by_id('educationClass-id').assignments_by_id('educationAssignment-id').submissions_by_id('educationSubmission-id').get(request_configuration)


```