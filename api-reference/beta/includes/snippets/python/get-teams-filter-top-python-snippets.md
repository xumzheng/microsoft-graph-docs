---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = TeamsRequestBuilderGetRequestConfiguration();

queryParameters = TeamsRequestBuilderGetQueryParameters();
queryParameters.filter = "startswith(displayName,%20'A')";
queryParameters.top = 2;

requestConfiguration.queryParameters = queryParameters;


graphServiceClient.teams().get(requestConfiguration);


```