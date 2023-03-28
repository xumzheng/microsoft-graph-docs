---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new AgentGroupsRequestBuilderGetRequestConfiguration();

$queryParameters = new AgentGroupsRequestBuilderGetQueryParameters();
$queryParameters.expand = ["agents","publishedResources"];

$requestConfiguration.queryParameters = $queryParameters;


$requestResult = $graphServiceClient.onPremisesPublishingProfilesById('onPremisesPublishingProfile-id').agentGroups().get($requestConfiguration);


```