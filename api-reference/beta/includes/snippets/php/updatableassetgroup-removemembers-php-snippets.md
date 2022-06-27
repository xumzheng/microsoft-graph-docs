---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new AssetsRequestBody();


$assetsArray = [];

$assetsassets1 = new UpdatableAsset();

$assetsassets1AdditionalData = [
	"@odata.type" => '#microsoft.graph.windowsUpdates.azureADDevice',
	"id" => 'String (identifier)',
];
$assetsassets1->setAdditionalData($assetsassets1AdditionalData);

$assetsArray []= $assetsassets1;
$requestRequestBody->setAssets($assetsArray);
$result =  $graphClient->admin()->windows()->updates()->updatableAssetsById('updatableAsset-id')->removeMembers()->post($requestRequestBody);


```