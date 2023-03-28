---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new UnenrollAssetsByIdPostRequestBody();
$requestBody.setUpdateCategory(new UpdateCategory('feature'));

$requestBody.setMemberEntityType('#microsoft.graph.windowsUpdates.azureADDevice');

$requestBody.setIds(['String', 'String', 'String', ]);



$graphServiceClient.admin().windows().updates().updatableAssets().windowsUpdatesUnenrollAssetsById().post($requestBody);


```