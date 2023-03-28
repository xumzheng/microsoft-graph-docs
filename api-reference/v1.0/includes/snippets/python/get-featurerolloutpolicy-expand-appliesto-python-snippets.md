---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new FeatureRolloutPolicyRequestBuilderGetRequestConfiguration();

$queryParameters = new FeatureRolloutPolicyRequestBuilderGetQueryParameters();
$queryParameters.expand = ["appliesTo"];

$requestConfiguration.queryParameters = $queryParameters;


$requestResult = $graphServiceClient.policies().featureRolloutPoliciesById('featureRolloutPolicy-id').get($requestConfiguration);


```