---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new OnPremisesPublishingProfileRequestBuilderGetRequestConfiguration();

$queryParameters = new OnPremisesPublishingProfileRequestBuilderGetQueryParameters();
$queryParameters.expand = ["publishedResources","agents","agentGroups"];

$requestConfiguration.queryParameters = $queryParameters;


$requestResult = $graphServiceClient.onPremisesPublishingProfilesById('onPremisesPublishingProfile-id').get($requestConfiguration);


```