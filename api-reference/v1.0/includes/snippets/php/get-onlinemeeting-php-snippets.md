---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new OnlineMeetingsRequestBuilderGetRequestConfiguration();

$queryParameters = new OnlineMeetingsRequestBuilderGetQueryParameters();
$queryParameters->filter = 'VideoTeleconferenceId%20eq%20\'123456789\'';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->communications()->onlineMeetings()->get($requestConfiguration);


```