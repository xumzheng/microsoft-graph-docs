---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = UpdatableAsset();
requestBody.set@odatatype('#microsoft.graph.windowsUpdates.updatableAssetGroup');



result = awaitclient.admin().windows().updates().updatableAssets().post(requestBody);


```