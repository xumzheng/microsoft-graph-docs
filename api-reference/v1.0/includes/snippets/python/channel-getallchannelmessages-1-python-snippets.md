---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = GetAllMessagesRequestBuilderGetRequestConfiguration(
query_params = GetAllMessagesRequestBuilderGetQueryParameters()
query_params.filter = "lastModifiedDateTime gt 2019-11-01T00:00:00Z and lastModifiedDateTime lt 2021-11-01T00:00:00Z"

)


result = await client.teams_by_id('team-id').channels.getAllMessages.get(request_config)


```