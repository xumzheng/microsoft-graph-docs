---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

request_config = ChannelsRequestBuilderGetRequestConfiguration();

query_params = ChannelsRequestBuilderGetQueryParameters();
query_params.filter = "membershipType eq 'private'";

request_config.queryParameters = query_params;


result = awaitclient.teamsById('team-id').channels().get(request_config);


```