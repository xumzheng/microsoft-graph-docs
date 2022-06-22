---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new EnrollAssetsPostRequestBody();


$requestRequestBody->setUpdateCategory(new UpdateCategory('String'));
$assetsArray = [];

$assets1 = new UpdatableAsset();

$assets1AdditionalData = [
		"@odata.type" => '#microsoft.graph.windowsUpdates.azureADDevice',
		"id" => 'String (identifier)',
	];
$assets1->setAdditionalData($assets1AdditionalData);

$assetsArray []= $assets1;
$requestRequestBody->setAssets($assetsArray);
$result =  $graphClient->admin()->windows()->updates()->updatableAssets()->enrollAssets()->post($requestRequestBody);


```