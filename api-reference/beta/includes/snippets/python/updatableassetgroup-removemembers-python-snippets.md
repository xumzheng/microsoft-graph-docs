---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = RemoveMembersPostRequestBody();
assetsUpdatableAsset1 = UpdatableAsset();
assetsUpdatableAsset1.set@odatatype('#microsoft.graph.windowsUpdates.azureADDevice');

assetsUpdatableAsset1.setId('String (identifier)');


assetsArray []= assetsUpdatableAsset1;
requestBody.setAssets(assetsArray);




awaitclient.admin().windows().updates().updatableAssetsById('updatableAsset-id').windowsUpdatesRemoveMembers().post(requestBody);


```