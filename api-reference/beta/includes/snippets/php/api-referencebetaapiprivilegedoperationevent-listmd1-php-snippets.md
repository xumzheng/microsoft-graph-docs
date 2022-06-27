---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new PrivilegedOperationEventsRequestBuilderGetRequestConfiguration();

$queryParameters = new PrivilegedOperationEventsRequestBuilderGetQueryParameters();
$queryParameters->filter = 'requestType%20eq%20\'Activate\'';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->privilegedOperationEvents()->get($requestConfiguration);


```