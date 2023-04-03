---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = MessagesRequestBuilderGetRequestConfiguration();

queryParameters = MessagesRequestBuilderGetQueryParameters();
queryParameters.filter = "Extensions/any";
queryParameters.expand = ["Extensions($filter=id%20eq%20'Com.Contoso.Referral')"];

requestConfiguration.queryParameters = queryParameters;


requestResult = graphServiceClient.me().messages().get(requestConfiguration);


```