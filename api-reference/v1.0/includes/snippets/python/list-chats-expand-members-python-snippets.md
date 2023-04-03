---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

request_config = ChatsRequestBuilderGetRequestConfiguration();

query_params = ChatsRequestBuilderGetQueryParameters();
query_params.expand = ["members"];

request_config.queryParameters = query_params;


result = awaitclient.usersById('user-id').chats().get(request_config);


```