---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

request_config = FeatureRolloutPolicyRequestBuilderGetRequestConfiguration();

query_params = FeatureRolloutPolicyRequestBuilderGetQueryParameters();
query_params.expand = ["appliesTo"];

request_config.queryParameters = query_params;


result = awaitclient.policies().featureRolloutPoliciesById('featureRolloutPolicy-id').get(request_config);


```