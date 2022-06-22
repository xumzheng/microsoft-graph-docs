---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new OnPremisesAgentGroupRequestBuilderGetRequestConfiguration();

$queryParameters = new OnPremisesAgentGroupRequestBuilderGetQueryParameters();
$queryParameters->expand = 'publishedResources,agents';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->onPremisesPublishingProfilesById('onPremisesPublishingProfile-id')->agentGroupsById('onPremisesAgentGroup-id')->get($requestConfiguration);


```