---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new AgentGroupsRequestBuilderGetRequestConfiguration();

$queryParameters = new AgentGroupsRequestBuilderGetQueryParameters();
$queryParameters->expand = 'agents,publishedResources';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->onPremisesPublishingProfilesById('onPremisesPublishingProfile-id')->agentGroups()->get($requestConfiguration);


```