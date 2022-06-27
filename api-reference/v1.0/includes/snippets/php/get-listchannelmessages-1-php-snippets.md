---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new MessagesRequestBuilderGetRequestConfiguration();

$queryParameters = new MessagesRequestBuilderGetQueryParameters();
$queryParameters->top = 3;

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->teamsById('team-id')->channelsById('channel-id')->messages()->get($requestConfiguration);


```