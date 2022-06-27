---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new SessionsRequestBuilderGetRequestConfiguration();

$queryParameters = new SessionsRequestBuilderGetQueryParameters();
$queryParameters->expand = 'segments';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->communications()->callRecordsById('callRecord-id')->sessions()->get($requestConfiguration);


```