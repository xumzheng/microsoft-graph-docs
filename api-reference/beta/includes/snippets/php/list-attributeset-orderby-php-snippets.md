---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new AttributeSetsRequestBuilderGetRequestConfiguration();

$queryParameters = new AttributeSetsRequestBuilderGetQueryParameters();
$queryParameters->orderBy = 'id';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->directory()->attributeSets()->get($requestConfiguration);


```