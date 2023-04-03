---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = TeamsRequestBuilderGetRequestConfiguration();

queryParameters = TeamsRequestBuilderGetQueryParameters();
queryParameters.filter = "displayName eq 'A Contoso Team'";
queryParameters.select = ["id","description"];

requestConfiguration.queryParameters = queryParameters;


graphServiceClient.teams().get(requestConfiguration);


```