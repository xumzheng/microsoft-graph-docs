---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = ChatRequestBuilderGetRequestConfiguration();

queryParameters = ChatRequestBuilderGetQueryParameters();
queryParameters.expand = ["members"];

requestConfiguration.queryParameters = queryParameters;


requestResult = graphServiceClient.chatsById('chat-id').get(requestConfiguration);


```