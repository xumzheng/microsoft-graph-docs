---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

request_config = OutcomesRequestBuilderGetRequestConfiguration();

query_params = OutcomesRequestBuilderGetQueryParameters();
query_params.filter = "isof('microsoft.graph.educationFeedbackResourceOutcome')";

request_config.queryParameters = query_params;


result = awaitclient.education().classesById('educationClass-id').assignmentsById('educationAssignment-id').submissionsById('educationSubmission-id').outcomes().get(request_config);


```