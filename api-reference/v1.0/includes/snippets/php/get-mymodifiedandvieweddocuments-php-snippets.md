---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new UsedRequestBuilderGetRequestConfiguration();

$queryParameters = new UsedRequestBuilderGetQueryParameters();
$queryParameters->orderby = 'LastUsed/LastAccessedDateTime%20desc';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->me()->insights()->used()->get($requestConfiguration);


```