---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_config = AllChannelsRequestBuilderGetRequestConfiguration();

query_params = AllChannelsRequestBuilderGetQueryParameters();
query_params.filter = "membershipType eq 'shared'";

request_config.queryParameters = query_params;


result = await client.teamsById('team-id').allChannels.get(request_config);


```