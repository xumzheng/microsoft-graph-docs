---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_config = AgentGroupsRequestBuilderGetRequestConfiguration();

query_params = AgentGroupsRequestBuilderGetQueryParameters();
query_params.expand = ["agents","publishedResources"];

request_config.queryParameters = query_params;


result = await client.onPremisesPublishingProfilesById('onPremisesPublishingProfile-id').agentGroups.get(request_config);


```