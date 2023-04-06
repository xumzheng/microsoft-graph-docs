---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = TeamsTabRequestBuilderGetRequestConfiguration(
request_config = TeamsTabRequestBuilderGetRequestConfiguration(query_params=params['expand'] = ["teamsApp"]
)


result = await client.chats_by_id('chat-id').tabs_by_id('teamsTab-id').get(request_config, headers=request_config)


```