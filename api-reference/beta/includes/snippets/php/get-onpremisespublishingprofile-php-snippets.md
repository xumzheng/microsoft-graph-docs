---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new OnPremisesPublishingProfileRequestBuilderGetRequestConfiguration();

$queryParameters = new OnPremisesPublishingProfileRequestBuilderGetQueryParameters();
$queryParameters->expand = 'publishedResources,agents,agentGroups';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->onPremisesPublishingProfilesById('onPremisesPublishingProfile-id')->get($requestConfiguration);


```