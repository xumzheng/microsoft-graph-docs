---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new PublishedResourceRequestBuilderGetRequestConfiguration();

$queryParameters = new PublishedResourceRequestBuilderGetQueryParameters();
$queryParameters->expand = 'agentGroups';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->onPremisesPublishingProfilesById('onPremisesPublishingProfile-id')->publishedResourcesById('publishedResource-id')->get($requestConfiguration);


```