---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = FeatureRolloutPolicy()
request_body.setDisplayName('PasswordHashSync Rollout Policy')

request_body.setDescription('PasswordHashSync Rollout Policy')

request_body.setIsEnabled(true)

request_body.setIsAppliedToOrganization(false)



result = await client.policies_featureRolloutPoliciesby_id('featureRolloutPolicy-id').patch(request_body)


```