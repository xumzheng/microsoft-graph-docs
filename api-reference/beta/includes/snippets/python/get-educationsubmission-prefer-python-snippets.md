---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = EducationSubmissionRequestBuilderGetRequestConfiguration();

headers = [
	'Prefer' => 'include-unknown-enum-members',
];

requestConfiguration.headers = headers;


requestResult = graphServiceClient.education().classesById('educationClass-id').assignmentsById('educationAssignment-id').submissionsById('educationSubmission-id').get(requestConfiguration);


```