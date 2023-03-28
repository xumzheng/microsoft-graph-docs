---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new FeatureRolloutPolicy();
$requestBody.setDisplayName('PassthroughAuthentication rollout policy');

$requestBody.setDescription('PassthroughAuthentication rollout policy');

$requestBody.setFeature(new StagedFeatureName('passthroughauthentication'));

$requestBody.setIsEnabled(true);

$requestBody.setIsAppliedToOrganization(false);



$requestResult = $graphServiceClient.policies().featureRolloutPolicies().post($requestBody);


```