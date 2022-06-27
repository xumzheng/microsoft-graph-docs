---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new FeatureRolloutPolicyRequestBuilderGetRequestConfiguration();

$queryParameters = new FeatureRolloutPolicyRequestBuilderGetQueryParameters();
$queryParameters->expand = 'appliesTo';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->policies()->featureRolloutPoliciesById('featureRolloutPolicy-id')->get($requestConfiguration);


```