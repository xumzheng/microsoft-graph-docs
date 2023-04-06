---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = TeamsTabRequestBuilderGetRequestConfiguration(
request_configuration = TeamsTabRequestBuilderGetRequestConfiguration(query_params=query_params = TeamsTabRequestBuilderGetQueryParameters()
query_params['expand'] = ["teamsApp"]

)
query_params = TeamsTabRequestBuilderGetQueryParameters()
query_params['expand'] = ["teamsApp"]

)


result = await client.chats_by_id('chat-id').tabs_by_id('teamsTab-id').get(request_configuration)


```