---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = UpdatableAsset()
request_body.set@odatatype('#microsoft.graph.windowsUpdates.updatableAssetGroup')



result = await client.admin.windows.updates.updatableAssets.post(request_body, headers=)


```