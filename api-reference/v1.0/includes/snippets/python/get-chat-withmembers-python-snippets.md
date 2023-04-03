---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

request_config = ChatRequestBuilderGetRequestConfiguration();

query_params = ChatRequestBuilderGetQueryParameters();
query_params.expand = ["members"];

request_config.queryParameters = query_params;


result = awaitclient.chatsById('chat-id').get(request_config);


```