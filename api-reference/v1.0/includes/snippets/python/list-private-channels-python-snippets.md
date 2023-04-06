---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = ChannelsRequestBuilderGetRequestConfiguration(
request_configuration = ChannelsRequestBuilderGetRequestConfiguration(query_params=query_params = ChannelsRequestBuilderGetQueryParameters()
query_params['filter'] = "membershipType eq 'private'"

)
query_params = ChannelsRequestBuilderGetQueryParameters()
query_params['filter'] = "membershipType eq 'private'"

)


result = await client.teams_by_id('team-id').channels.get(request_configuration)


```