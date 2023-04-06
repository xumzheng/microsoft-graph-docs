---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = FeatureRolloutPolicyRequestBuilderGetRequestConfiguration(
request_configuration = FeatureRolloutPolicyRequestBuilderGetRequestConfiguration(query_params=query_params = FeatureRolloutPolicyRequestBuilderGetQueryParameters()
query_params['expand'] = ["appliesTo"]

)
query_params = FeatureRolloutPolicyRequestBuilderGetQueryParameters()
query_params['expand'] = ["appliesTo"]

)


result = await client.policies.featureRolloutPolicies_by_id('featureRolloutPolicy-id').get(request_configuration)


```