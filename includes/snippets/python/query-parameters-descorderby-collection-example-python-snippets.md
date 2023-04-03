---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = MessagesRequestBuilderGetRequestConfiguration();

queryParameters = MessagesRequestBuilderGetQueryParameters();
queryParameters.orderby = ["from/emailAddress/name desc","subject"];

requestConfiguration.queryParameters = queryParameters;


requestResult = graphServiceClient.me().mailFoldersById('mailFolder-id').messages().get(requestConfiguration);


```