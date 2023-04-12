---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = EnrollAssetsByIdPostRequestBody()
request_body.UpdateCategory(UpdateCategory('feature'))

request_body.memberEntityType = '#microsoft.graph.windowsUpdates.azureADDevice'

request_body.Ids(['String', 'String', 'String', ])




await client.admin.windows.updates.updatableAssets.windowsUpdatesenrollAssetsById.post(request_body = request_body)


```