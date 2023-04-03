---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = IncidentsRequestBuilderGetRequestConfiguration();

queryParameters = IncidentsRequestBuilderGetQueryParameters();
queryParameters.expand = ["alerts"];

requestConfiguration.queryParameters = queryParameters;


requestResult = graphServiceClient.security().incidents().get(requestConfiguration);


```