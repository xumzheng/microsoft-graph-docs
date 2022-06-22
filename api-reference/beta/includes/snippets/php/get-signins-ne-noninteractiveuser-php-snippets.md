---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new SignInsRequestBuilderGetRequestConfiguration();

$queryParameters = new SignInsRequestBuilderGetQueryParameters();
$queryParameters->filter = '(signInEventTypes/any)';
$queryParameters->orderBy = 'createdDateTime%20DESC';
$queryParameters->top = 10;

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->auditLogs()->signIns()->get($requestConfiguration);


```