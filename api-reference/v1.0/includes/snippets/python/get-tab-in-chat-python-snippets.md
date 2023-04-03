---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

request_config = TeamsTabRequestBuilderGetRequestConfiguration();

query_params = TeamsTabRequestBuilderGetQueryParameters();
query_params.expand = ["teamsApp"];

request_config.queryParameters = query_params;


result = awaitclient.chatsById('chat-id').tabsById('teamsTab-id').get(request_config);


```