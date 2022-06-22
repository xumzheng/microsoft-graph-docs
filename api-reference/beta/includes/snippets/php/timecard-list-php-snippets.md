---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new TimeCardsRequestBuilderGetRequestConfiguration();

$queryParameters = new TimeCardsRequestBuilderGetQueryParameters();
$queryParameters->top = 2;
$queryParameters->filter = 'state%20eq%20\'clockedOut\'';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->teamsById('team-id')->schedule()->timeCards()->get($requestConfiguration);


```