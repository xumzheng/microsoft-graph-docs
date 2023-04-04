---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_config = MessagesRequestBuilderGetRequestConfiguration();

query_params = MessagesRequestBuilderGetQueryParameters;
query_params.top = 1;
query_params.expand = ["replies"];

request_config.queryParameters = query_params;


result = await client.teamsById('team-id').channelsById('channel-id').messages().get(request_config);


```