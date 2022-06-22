---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new FeatureRolloutPolicy();


$requestRequestBody->setDisplayName('PassthroughAuthentication rollout policy');
$requestRequestBody->setDescription('PassthroughAuthentication rollout policy');
$requestRequestBody->setFeature(new StagedFeatureName('passthroughAuthentication'));
$requestRequestBody->setIsEnabled(True);
$requestRequestBody->setIsAppliedToOrganization(False);
$result =  $graphClient->policies()->featureRolloutPolicies()->post($requestRequestBody);


```