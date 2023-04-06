---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = TabsRequestBuilderGetRequestConfiguration(
request_config = TabsRequestBuilderGetRequestConfiguration(query_params=query_params = TabsRequestBuilderGetQueryParameters()
query_params.expand = ["teamsApp"]
query_params.filter = "teamsApp/id eq 'com.microsoft.teamspace.tab.web'"

)
query_params = TabsRequestBuilderGetQueryParameters()
query_params.expand = ["teamsApp"]
query_params.filter = "teamsApp/id eq 'com.microsoft.teamspace.tab.web'"

)


result = await client.chats_by_id('chat-id').tabs.get(request_config, headers=request_config)


```