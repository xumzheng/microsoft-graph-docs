---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new SecureScoresRequestBuilderGetRequestConfiguration();

$queryParameters = new SecureScoresRequestBuilderGetQueryParameters();
$queryParameters->top = 1;

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->security()->secureScores()->get($requestConfiguration);


```