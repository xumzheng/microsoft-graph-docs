---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = ChannelsRequestBuilderGetRequestConfiguration()

query_params = ChannelsRequestBuilderGetQueryParameters()
query_params.filter = "membershipType eq 'shared'"

request_config.queryParameters = query_params


result = await client.teams_by_id('team-id').channels.get(request_config)


```