---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new PublishedResourcesRequestBuilderGetRequestConfiguration();

$queryParameters = new PublishedResourcesRequestBuilderGetQueryParameters();
$queryParameters->expand = ["agentGroups"];

$requestConfiguration->queryParameters = $queryParameters;


$requestResult = $graphServiceClient->onPremisesPublishingProfilesById('onPremisesPublishingProfile-id')->publishedResources()->get($requestConfiguration);


```