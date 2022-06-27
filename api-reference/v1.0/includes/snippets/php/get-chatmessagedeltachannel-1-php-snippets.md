---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new DeltaRequestBuilderGetRequestConfiguration();

$queryParameters = new DeltaRequestBuilderGetQueryParameters();
$queryParameters->top = 2;

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->teamsById('team-id')->channelsById('channel-id')->messages()->delta()()->get($requestConfiguration);


```