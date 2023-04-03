---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = MessagesRequestBuilderGetRequestConfiguration();

queryParameters = MessagesRequestBuilderGetQueryParameters();
queryParameters.filter = "subject eq 'let''s meet for lunch?'";

requestConfiguration.queryParameters = queryParameters;


requestResult = graphServiceClient.me().messages().get(requestConfiguration);


```