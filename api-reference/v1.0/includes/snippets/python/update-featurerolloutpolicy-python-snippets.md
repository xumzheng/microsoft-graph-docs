---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new FeatureRolloutPolicy();
$requestBody.setDisplayName('PasswordHashSync Rollout Policy');

$requestBody.setDescription('PasswordHashSync Rollout Policy');

$requestBody.setIsEnabled(true);

$requestBody.setIsAppliedToOrganization(false);



$requestResult = $graphServiceClient.policies().featureRolloutPoliciesById('featureRolloutPolicy-id').patch($requestBody);


```