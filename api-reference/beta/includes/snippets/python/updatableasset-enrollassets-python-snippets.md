---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = EnrollAssetsPostRequestBody()
request_body.setUpdateCategory(UpdateCategory('string'))

assetsUpdatableAsset1 = UpdatableAsset()
assetsUpdatableAsset1.set@odatatype('#microsoft.graph.windowsUpdates.azureADDevice')

assetsUpdatableAsset1.setId('String (identifier)')


assetsArray []= assetsUpdatableAsset1;
request_body.setAssets(assetsArray)



request_config = EnrollAssetsRequestBuilderPostRequestConfiguration(
request_config = EnrollAssetsRequestBuilderPostRequestConfiguration(query_params=)


await client.admin.windows.updates.updatableAssets.windowsUpdatesenrollAssets.post(request_body, headers=)


```