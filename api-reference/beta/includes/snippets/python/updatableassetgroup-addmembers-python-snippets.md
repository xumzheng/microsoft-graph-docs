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



request_config = AddMembersRequestBuilderPostRequestConfiguration(
request_config = AddMembersRequestBuilderPostRequestConfiguration(query_params=)


await client.admin.windows.updates.updatableAssets_by_id('updatableAsset-id').windowsUpdatesaddMembers.post(request_body, headers=)


```