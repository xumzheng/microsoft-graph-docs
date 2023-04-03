---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = SubmissionsRequestBuilderGetRequestConfiguration();

queryParameters = SubmissionsRequestBuilderGetQueryParameters();
queryParameters.expand = ["outcomes"];

requestConfiguration.queryParameters = queryParameters;


requestResult = graphServiceClient.education().classesById('educationClass-id').assignmentsById('educationAssignment-id').submissions().get(requestConfiguration);


```