---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = ServicePrincipalsRequestBuilderGetRequestConfiguration();

queryParameters = ServicePrincipalsRequestBuilderGetQueryParameters();
queryParameters.filter = "appId eq '00000002-0000-0000-c000-000000000000'";

requestConfiguration.queryParameters = queryParameters;


requestResult = graphServiceClient.servicePrincipals().get(requestConfiguration);


```