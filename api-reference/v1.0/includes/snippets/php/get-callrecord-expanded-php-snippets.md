---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new CallRecordRequestBuilderGetRequestConfiguration();

$queryParameters = new CallRecordRequestBuilderGetQueryParameters();
$queryParameters->expand = 'sessions($expand=segments)';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->communications()->callRecordsById('callRecord-id')->get($requestConfiguration);


```