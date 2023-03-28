---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new UnenrollAssetsPostRequestBody();
$requestBody->setUpdateCategory(new UpdateCategory('string'));

$assetsUpdatableAsset1 = new UpdatableAsset();
$assetsUpdatableAsset1->set@odatatype('#microsoft.graph.windowsUpdates.azureADDevice');

$assetsUpdatableAsset1->setId('String (identifier)');


$assetsArray []= $assetsUpdatableAsset1;
$requestBody->setAssets($assetsArray);




$graphServiceClient->admin()->windows()->updates()->updatableAssets()->windowsUpdatesUnenrollAssets()->post($requestBody);


```