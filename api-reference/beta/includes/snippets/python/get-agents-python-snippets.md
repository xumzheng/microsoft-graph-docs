---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

request_config = AgentsRequestBuilderGetRequestConfiguration();

query_params = AgentsRequestBuilderGetQueryParameters();
query_params.expand = ["agentGroups"];

request_config.queryParameters = query_params;


result = awaitclient.onPremisesPublishingProfilesById('onPremisesPublishingProfile-id').agents().get(request_config);


```