---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = RemoveMembersByIdPostRequestBody();
requestBody.setIds(['String', 'String', 'String', ]);

requestBody.setMemberEntityType('#microsoft.graph.windowsUpdates.azureADDevice');



awaitclient.admin().windows().updates().updatableAssetsById('updatableAsset-id').windowsUpdatesRemoveMembersById().post(requestBody);


```