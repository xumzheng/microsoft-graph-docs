---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new GroupsRequestBuilderGetRequestConfiguration();

$queryParameters = new GroupsRequestBuilderGetQueryParameters();
$queryParameters->select = 'id,assignedLicenses';
$queryParameters->filter = 'assignedLicenses/any()';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->groups()->get($requestConfiguration);


```