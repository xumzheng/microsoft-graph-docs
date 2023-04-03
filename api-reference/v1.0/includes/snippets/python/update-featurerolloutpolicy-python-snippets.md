---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = FeatureRolloutPolicy();
requestBody.setDisplayName('PasswordHashSync Rollout Policy');

requestBody.setDescription('PasswordHashSync Rollout Policy');

requestBody.setIsEnabled(true);

requestBody.setIsAppliedToOrganization(false);



result = await client.policies().featureRolloutPoliciesById('featureRolloutPolicy-id').patch(requestBody);


```