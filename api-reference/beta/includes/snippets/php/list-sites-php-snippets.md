---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new SitesRequestBuilderGetRequestConfiguration();

$queryParameters = new SitesRequestBuilderGetQueryParameters();
$queryParameters->select = 'siteCollection,webUrl';
$queryParameters->filter = 'siteCollection/root%20ne%20null';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->sites()->get($requestConfiguration);


```