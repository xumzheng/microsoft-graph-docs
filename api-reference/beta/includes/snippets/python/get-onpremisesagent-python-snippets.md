---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new OnPremisesAgentRequestBuilderGetRequestConfiguration();

$queryParameters = new OnPremisesAgentRequestBuilderGetQueryParameters();
$queryParameters.expand = ["agentGroups"];

$requestConfiguration.queryParameters = $queryParameters;


$requestResult = $graphServiceClient.onPremisesPublishingProfilesById('onPremisesPublishingProfile-id').agentsById('onPremisesAgent-id').get($requestConfiguration);


```