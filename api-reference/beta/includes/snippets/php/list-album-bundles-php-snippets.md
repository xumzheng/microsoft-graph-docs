---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new BundlesRequestBuilderGetRequestConfiguration();

$queryParameters = new BundlesRequestBuilderGetQueryParameters();
$queryParameters->filter = 'bundle/album%20ne%20null';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->drive()->bundles()->get($requestConfiguration);


```