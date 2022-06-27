---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new EnrollAssetsPostRequestBody();


$requestRequestBody->setUpdateCategory(new UpdateCategory('String'));
$assetsArray = [];

$assetsassets1 = new UpdatableAsset();

$assetsassets1AdditionalData = [
	"@odata.type" => '#microsoft.graph.windowsUpdates.azureADDevice',
	"id" => 'String (identifier)',
];
$assetsassets1->setAdditionalData($assetsassets1AdditionalData);

$assetsArray []= $assetsassets1;
$requestRequestBody->setAssets($assetsArray);
$result =  $graphClient->admin()->windows()->updates()->updatableAssets()->enrollAssets()->post($requestRequestBody);


```