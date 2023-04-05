---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = EnrollAssetsByIdPostRequestBody()
request_body.setUpdateCategory(UpdateCategory('feature'))

request_body.setMemberEntityType('#microsoft.graph.windowsUpdates.azureADDevice')

request_body.setIds(['String', 'String', 'String', ])



await client.admin_windows_updates_updatableAssets_windowsUpdatesenrollAssetsById.post(request_body)


```