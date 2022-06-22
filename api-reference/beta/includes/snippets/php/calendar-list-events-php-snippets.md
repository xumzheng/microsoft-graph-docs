---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new EventsRequestBuilderGetRequestConfiguration();

$queryParameters = new EventsRequestBuilderGetQueryParameters();
$queryParameters->filter = 'startsWith(subject,\'All\')';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->me()->calendar()->events()->get($requestConfiguration);


```