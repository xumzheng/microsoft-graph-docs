---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = RemoveMembersPostRequestBody();
assetsUpdatableAsset1 = UpdatableAsset();
assetsUpdatableAsset1.set@odatatype('#microsoft.graph.windowsUpdates.azureADDevice');

assetsUpdatableAsset1.setId('String (identifier)');


assetsArray []= assetsUpdatableAsset1;
requestBody.setAssets(assetsArray);




graphServiceClient.admin().windows().updates().updatableAssetsById('updatableAsset-id').windowsUpdatesRemoveMembers().post(requestBody);


```