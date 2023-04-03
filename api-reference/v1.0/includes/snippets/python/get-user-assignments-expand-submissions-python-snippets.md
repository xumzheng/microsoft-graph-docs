---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = AssignmentsRequestBuilderGetRequestConfiguration();

queryParameters = AssignmentsRequestBuilderGetQueryParameters();
queryParameters.expand = ["submissions"];

requestConfiguration.queryParameters = queryParameters;


requestResult = graphServiceClient.education().usersById('educationUser-id').assignments().get(requestConfiguration);


```