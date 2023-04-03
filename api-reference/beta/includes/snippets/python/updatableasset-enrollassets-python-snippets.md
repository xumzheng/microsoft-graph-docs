---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = EnrollAssetsPostRequestBody();
requestBody.setUpdateCategory(UpdateCategory('string'));

assetsUpdatableAsset1 = UpdatableAsset();
assetsUpdatableAsset1.set@odatatype('#microsoft.graph.windowsUpdates.azureADDevice');

assetsUpdatableAsset1.setId('String (identifier)');


assetsArray []= assetsUpdatableAsset1;
requestBody.setAssets(assetsArray);




await client.admin().windows().updates().updatableAssets().windowsUpdatesEnrollAssets().post(requestBody);


```