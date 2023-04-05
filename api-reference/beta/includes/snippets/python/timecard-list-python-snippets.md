---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = TimeCardsRequestBuilderGetRequestConfiguration()

query_params = TimeCardsRequestBuilderGetQueryParameters()
query_params.top = 2
query_params.filter = "state eq 'clockedOut'"

request_config.queryParameters = query_params


result = await client.teamsby_id('team-id')_schedule_timeCards.get(request_config)


```