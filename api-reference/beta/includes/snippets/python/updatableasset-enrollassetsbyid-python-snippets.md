---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = EnrollAssetsByIdPostRequestBody();
requestBody.setUpdateCategory(UpdateCategory('feature'));

requestBody.setMemberEntityType('#microsoft.graph.windowsUpdates.azureADDevice');

requestBody.setIds(['String', 'String', 'String', ]);



graphServiceClient.admin().windows().updates().updatableAssets().windowsUpdatesEnrollAssetsById().post(requestBody);


```