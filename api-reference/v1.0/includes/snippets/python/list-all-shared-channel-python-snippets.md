---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = AllChannelsRequestBuilderGetRequestConfiguration(
request_config = AllChannelsRequestBuilderGetRequestConfiguration(query_params=query_params = AllChannelsRequestBuilderGetQueryParameters()
query_params.filter = "membershipType eq 'shared'"

)
query_params = AllChannelsRequestBuilderGetQueryParameters()
query_params.filter = "membershipType eq 'shared'"

)


result = await client.teams_by_id('team-id').allChannels.get(request_config, headers=request_config)


```