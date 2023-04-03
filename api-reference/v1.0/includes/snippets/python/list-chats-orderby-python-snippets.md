---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = ChatsRequestBuilderGetRequestConfiguration();

queryParameters = ChatsRequestBuilderGetQueryParameters();
queryParameters.orderby = ["lastMessagePreview/createdDateTime desc"];

requestConfiguration.queryParameters = queryParameters;


requestResult = graphServiceClient.chats().get(requestConfiguration);


```