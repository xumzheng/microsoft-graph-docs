---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new ContactsRequestBuilderGetRequestConfiguration();

$queryParameters = new ContactsRequestBuilderGetQueryParameters();
$queryParameters->search = '%22displayName:wa%22';
$queryParameters->count = true;

$headers = [
"ConsistencyLevel" => "eventual",
];

$requestConfiguration->queryParameters = $queryParameters;
$requestConfiguration->headers = $headers;


$result =  $graphClient->contacts()->get($requestConfiguration);


```