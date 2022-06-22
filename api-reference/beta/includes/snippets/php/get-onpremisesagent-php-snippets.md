---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new OnPremisesAgentRequestBuilderGetRequestConfiguration();

$queryParameters = new OnPremisesAgentRequestBuilderGetQueryParameters();
$queryParameters->expand = 'agentGroups';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->onPremisesPublishingProfilesById('onPremisesPublishingProfile-id')->agentsById('onPremisesAgent-id')->get($requestConfiguration);


```