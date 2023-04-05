---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AddMembersPostRequestBody()
assetsUpdatableAsset1 = UpdatableAsset()
assetsUpdatableAsset1.set@odatatype('#microsoft.graph.windowsUpdates.azureADDevice')

assetsUpdatableAsset1.setId('String (identifier)')


assetsArray []= assetsUpdatableAsset1;
request_body.setAssets(assetsArray)




await client.admin.windows.updates.updatableAssetsById('updatableAsset-id').windowsUpdatesaddMembers.post(request_body)


```