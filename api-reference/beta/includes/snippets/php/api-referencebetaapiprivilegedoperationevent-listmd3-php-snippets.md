---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new PrivilegedOperationEventsRequestBuilderGetRequestConfiguration();

$queryParameters = new PrivilegedOperationEventsRequestBuilderGetQueryParameters();
$queryParameters->filter = '(creationDateTime%20ge%202017-06-25T07:00:00Z)%20and%20';
$queryParameters->count = true;
$queryParameters->orderby = 'creationDateTime%20desc';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->privilegedOperationEvents()->get($requestConfiguration);


```