---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = FeatureRolloutPolicy()
request_body.setDisplayName('PassthroughAuthentication rollout policy')

request_body.setDescription('PassthroughAuthentication rollout policy')

request_body.setFeature(StagedFeatureName('passthroughauthentication'))

request_body.setIsEnabled(true)

request_body.setIsAppliedToOrganization(false)


request_config = FeatureRolloutPoliciesRequestBuilderPostRequestConfiguration(
request_config = FeatureRolloutPoliciesRequestBuilderPostRequestConfiguration(query_params=)


result = await client.policies.featureRolloutPolicies.post(request_body, headers=)


```