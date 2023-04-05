---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = TabsRequestBuilderGetRequestConfiguration()

query_params = TabsRequestBuilderGetQueryParameters()
query_params.expand = ["teamsApp"]
query_params.filter = "teamsApp/id eq 'com.microsoft.teamspace.tab.planner'"

request_config.queryParameters = query_params


result = await client.teamsby_id('team-id')_channelsby_id('channel-id')_tabs.get(request_config)


```