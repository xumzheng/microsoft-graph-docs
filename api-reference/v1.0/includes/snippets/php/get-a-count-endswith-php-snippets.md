---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new UsersRequestBuilderGetRequestConfiguration();

$queryParameters = new UsersRequestBuilderGetQueryParameters();
$queryParameters->filter = 'endswith(mail,\'a@contoso.com\')';
$queryParameters->orderby = 'userPrincipalName';
$queryParameters->count = true;

$headers = [
"ConsistencyLevel" => "eventual",
];

$requestConfiguration->queryParameters = $queryParameters;
$requestConfiguration->headers = $headers;


$result =  $graphClient->users()->get($requestConfiguration);


```