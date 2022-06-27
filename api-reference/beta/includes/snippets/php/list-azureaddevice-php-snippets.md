---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new UpdatableAssetsRequestBuilderGetRequestConfiguration();

$queryParameters = new UpdatableAssetsRequestBuilderGetQueryParameters();
$queryParameters->filter = 'isof(\'microsoft.graph.windowsUpdates.azureADDevice\')';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->admin()->windows()->updates()->updatableAssets()->get($requestConfiguration);


```