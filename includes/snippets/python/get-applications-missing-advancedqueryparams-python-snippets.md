---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = ApplicationsRequestBuilderGetRequestConfiguration();

queryParameters = ApplicationsRequestBuilderGetQueryParameters();
queryParameters.search = "\"displayName:Browser\"";

requestConfiguration.queryParameters = queryParameters;


requestResult = graphServiceClient.applications().get(requestConfiguration);


```