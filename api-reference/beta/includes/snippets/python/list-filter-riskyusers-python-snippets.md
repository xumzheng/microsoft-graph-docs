---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = RiskyUsersRequestBuilderGetRequestConfiguration();

queryParameters = RiskyUsersRequestBuilderGetQueryParameters();
queryParameters.filter = "riskLevel eq microsoft.graph.riskLevel'medium'";

requestConfiguration.queryParameters = queryParameters;


requestResult = graphServiceClient.identityProtection().riskyUsers().get(requestConfiguration);


```