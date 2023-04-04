---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_config = EducationSubmissionRequestBuilderGetRequestConfiguration()

headers = [
	'Prefer' => 'include-unknown-enum-members',
]

request_config.headers = headers


result = await client.education.classesById('educationClass-id').assignmentsById('educationAssignment-id').submissionsById('educationSubmission-id').get(request_config)


```