---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = FeatureRolloutPolicy()
request_body.displayName = 'PassthroughAuthentication rollout policy'

request_body.description = 'PassthroughAuthentication rollout policy'

request_body.Feature(StagedFeatureName('passthroughauthentication'))

request_body.isEnabled = true

request_body.isAppliedToOrganization = false



request_configuration = FeatureRolloutPoliciesRequestBuilderPostRequestConfiguration(
)


result = await client.policies.featureRolloutPolicies.post(request_body = request_body)


```