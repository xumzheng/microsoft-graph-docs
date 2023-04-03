---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = FeatureRolloutPolicy();
requestBody.setDisplayName('PassthroughAuthentication rollout policy');

requestBody.setDescription('PassthroughAuthentication rollout policy');

requestBody.setFeature(StagedFeatureName('passthroughauthentication'));

requestBody.setIsEnabled(true);

requestBody.setIsAppliedToOrganization(false);



result = awaitclient.policies().featureRolloutPolicies().post(requestBody);


```