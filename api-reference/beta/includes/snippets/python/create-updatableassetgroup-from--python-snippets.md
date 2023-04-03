---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = UpdatableAsset();
requestBody.set@odatatype('#microsoft.graph.windowsUpdates.updatableAssetGroup');



result = await client.admin().windows().updates().updatableAssets().post(requestBody);


```