---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = UnenrollAssetsByIdPostRequestBody();
requestBody.setUpdateCategory(UpdateCategory('feature'));

requestBody.setMemberEntityType('#microsoft.graph.windowsUpdates.azureADDevice');

requestBody.setIds(['String', 'String', 'String', ]);



awaitclient.admin().windows().updates().updatableAssets().windowsUpdatesUnenrollAssetsById().post(requestBody);


```