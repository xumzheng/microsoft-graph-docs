---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = UnenrollAssetsPostRequestBody()
request_body.UpdateCategory(UpdateCategory('string'))

assetsUpdatableAsset1 = UpdatableAsset()
assetsUpdatableAsset1.@odatatype = '#microsoft.graph.windowsUpdates.azureADDevice'

assetsUpdatableAsset1.id = 'String (identifier)'


assetsArray []= assetsUpdatableAsset1;
request_body.assets(assetsArray)




request_configuration = UnenrollAssetsRequestBuilderPostRequestConfiguration(
)


await client.admin.windows.updates.updatableAssets.windowsUpdatesunenrollAssets.post(request_body = request_body)


```