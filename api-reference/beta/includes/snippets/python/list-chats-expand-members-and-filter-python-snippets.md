---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_config = ChatsRequestBuilderGetRequestConfiguration();

query_params = ChatsRequestBuilderGetQueryParameters;
query_params.expand = ["members"];
query_params.filter = "members/any";

request_config.queryParameters = query_params;


result = await client.usersById('user-id').chats().get(request_config);


```