---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = EducationSubmissionRequestBuilderGetRequestConfiguration();

queryParameters = EducationSubmissionRequestBuilderGetQueryParameters();
queryParameters.expand = ["*"];

requestConfiguration.queryParameters = queryParameters;


requestResult = graphServiceClient.education().classesById('educationClass-id').assignmentsById('educationAssignment-id').submissionsById('educationSubmission-id').get(requestConfiguration);


```