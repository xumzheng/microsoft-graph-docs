---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

request_config = SubmissionsRequestBuilderGetRequestConfiguration();

query_params = SubmissionsRequestBuilderGetQueryParameters();
query_params.expand = ["outcomes"];

request_config.queryParameters = query_params;


result = awaitclient.education().classesById('educationClass-id').assignmentsById('educationAssignment-id').submissions().get(request_config);


```