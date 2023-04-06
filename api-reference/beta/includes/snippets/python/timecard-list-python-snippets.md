---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = TimeCardsRequestBuilderGetRequestConfiguration(
request_config = TimeCardsRequestBuilderGetRequestConfiguration(query_params=query_params = TimeCardsRequestBuilderGetQueryParameters()
query_params.top = 2
query_params.filter = "state eq 'clockedOut'"

)
query_params = TimeCardsRequestBuilderGetQueryParameters()
query_params.top = 2
query_params.filter = "state eq 'clockedOut'"

)


result = await client.teams_by_id('team-id').schedule.timeCards.get(request_config, headers=request_config)


```