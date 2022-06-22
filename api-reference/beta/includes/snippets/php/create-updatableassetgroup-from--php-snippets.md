---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new UpdatableAsset();


$requestRequestBodyAdditionalData = [
	"@odata.type" => '#microsoft.graph.windowsUpdates.updatableAssetGroup',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->admin()->windows()->updates()->updatableAssets()->post($requestRequestBody);


```