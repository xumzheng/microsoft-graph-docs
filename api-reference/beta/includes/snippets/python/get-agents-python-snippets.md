---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new AgentsRequestBuilderGetRequestConfiguration();

$queryParameters = new AgentsRequestBuilderGetQueryParameters();
$queryParameters.expand = ["agentGroups"];

$requestConfiguration.queryParameters = $queryParameters;


$requestResult = $graphServiceClient.onPremisesPublishingProfilesById('onPremisesPublishingProfile-id').agents().get($requestConfiguration);


```