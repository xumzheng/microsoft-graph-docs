---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = TabsRequestBuilderGetRequestConfiguration()

query_params = TabsRequestBuilderGetQueryParameters()
query_params.expand = ["teamsApp"]

request_config.queryParameters = query_params


result = await client.teamsById('team-id').channelsById('channel-id').tabs.get(request_config)


```