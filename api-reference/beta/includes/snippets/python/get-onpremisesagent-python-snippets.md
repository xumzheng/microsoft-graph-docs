---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_config = OnPremisesAgentRequestBuilderGetRequestConfiguration();

query_params = OnPremisesAgentRequestBuilderGetQueryParameters;
query_params.expand = ["agentGroups"];

request_config.queryParameters = query_params;


result = await client.onPremisesPublishingProfilesById('onPremisesPublishingProfile-id').agentsById('onPremisesAgent-id').get(request_config);


```