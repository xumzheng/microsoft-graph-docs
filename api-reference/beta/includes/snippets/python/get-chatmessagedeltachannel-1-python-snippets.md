---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = DeltaRequestBuilderGetRequestConfiguration(
request_configuration = DeltaRequestBuilderGetRequestConfiguration(query_params=query_params = DeltaRequestBuilderGetQueryParameters()
query_params['top'] = 2

)
query_params = DeltaRequestBuilderGetQueryParameters()
query_params['top'] = 2

)


result = await client.teams_by_id('team-id').channels_by_id('channel-id').messages.delta.get(request_configuration)


```