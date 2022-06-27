---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new PublishedResourcesRequestBuilderGetRequestConfiguration();

$queryParameters = new PublishedResourcesRequestBuilderGetQueryParameters();
$queryParameters->expand = 'agentGroups';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->onPremisesPublishingProfilesById('onPremisesPublishingProfile-id')->publishedResources()->get($requestConfiguration);


```