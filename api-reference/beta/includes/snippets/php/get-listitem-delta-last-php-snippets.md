---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new DeltaRequestBuilderGetRequestConfiguration();

$queryParameters = new DeltaRequestBuilderGetQueryParameters();
$queryParameters->token = '1230919asd190410jlka';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->sitesById('site-id')->listsById('list-id')->items()->delta()()->get($requestConfiguration);


```