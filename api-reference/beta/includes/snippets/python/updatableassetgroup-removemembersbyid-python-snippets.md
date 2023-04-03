---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = RemoveMembersByIdPostRequestBody();
requestBody.setIds(['String', 'String', 'String', ]);

requestBody.setMemberEntityType('#microsoft.graph.windowsUpdates.azureADDevice');



await client.admin().windows().updates().updatableAssetsById('updatableAsset-id').windowsUpdatesRemoveMembersById().post(requestBody);


```