---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = FeatureRolloutPolicy();
requestBody.setDisplayName('PassthroughAuthentication rollout policy');

requestBody.setDescription('PassthroughAuthentication rollout policy');

requestBody.setFeature(StagedFeatureName('passthroughauthentication'));

requestBody.setIsEnabled(true);

requestBody.setIsAppliedToOrganization(false);



result = await client.policies().featureRolloutPolicies().post(requestBody);


```