---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = UnenrollAssetsByIdPostRequestBody();
requestBody.setUpdateCategory(UpdateCategory('feature'));

requestBody.setMemberEntityType('#microsoft.graph.windowsUpdates.azureADDevice');

requestBody.setIds(['String', 'String', 'String', ]);



await client.admin().windows().updates().updatableAssets().windowsUpdatesUnenrollAssetsById().post(requestBody);


```