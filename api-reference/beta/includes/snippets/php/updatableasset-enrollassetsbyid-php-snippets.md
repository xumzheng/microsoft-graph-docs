---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new EnrollAssetsByIdPostRequestBody();


$requestRequestBody->setUpdateCategory(new UpdateCategory('feature'));
$requestRequestBody->setMemberEntityType('#microsoft.graph.windowsUpdates.azureADDevice');
$requestRequestBody->setIds( [
'String','String','String',],
$result =  $graphClient->admin()->windows()->updates()->updatableAssets()->enrollAssetsById()->post($requestRequestBody);


```