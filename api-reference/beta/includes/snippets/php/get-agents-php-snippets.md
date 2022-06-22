---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new AgentsRequestBuilderGetRequestConfiguration();

$queryParameters = new AgentsRequestBuilderGetQueryParameters();
$queryParameters->expand = 'agentGroups';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->onPremisesPublishingProfilesById('onPremisesPublishingProfile-id')->agents()->get($requestConfiguration);


```