---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = TabsRequestBuilderGetRequestConfiguration()

query_params = TabsRequestBuilderGetQueryParameters()
query_params.expand = ["teamsApp"]
query_params.filter = "teamsApp/id eq 'com.microsoft.teamspace.tab.web'"

request_config.queryParameters = query_params


result = await client.chatsby_id('chat-id')_tabs.get(request_config)


```