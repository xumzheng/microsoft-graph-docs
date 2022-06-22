---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new FeatureRolloutPolicy();


$requestRequestBody->setDisplayName('PasswordHashSync Rollout Policy');
$requestRequestBody->setDescription('PasswordHashSync Rollout Policy');
$requestRequestBody->setIsEnabled(True);
$requestRequestBody->setIsAppliedToOrganization(False);
$result =  $graphClient->policies()->featureRolloutPoliciesById('featureRolloutPolicy-id')->patch($requestRequestBody);


```