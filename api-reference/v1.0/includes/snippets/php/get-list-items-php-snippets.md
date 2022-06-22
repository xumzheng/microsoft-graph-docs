---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new ItemsRequestBuilderGetRequestConfiguration();

$queryParameters = new ItemsRequestBuilderGetQueryParameters();
$queryParameters->expand = 'fields(select=Name,Color,Quantity)';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->sitesById('site-id')->listsById('list-id')->items()->get($requestConfiguration);


```