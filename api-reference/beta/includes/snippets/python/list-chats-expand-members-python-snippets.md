---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = ChatsRequestBuilderGetRequestConfiguration();

queryParameters = ChatsRequestBuilderGetQueryParameters();
queryParameters.expand = ["members"];

requestConfiguration.queryParameters = queryParameters;


requestResult = graphServiceClient.usersById('user-id').chats().get(requestConfiguration);


```