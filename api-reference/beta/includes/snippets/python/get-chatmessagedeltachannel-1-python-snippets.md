---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_config = DeltaRequestBuilderGetRequestConfiguration();

query_params = DeltaRequestBuilderGetQueryParameters();
query_params.top = 2;

request_config.queryParameters = query_params;


result = await client.teamsById('team-id').channelsById('channel-id').messages().delta().get(request_config);


```