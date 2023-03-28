---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new RemoveMembersByIdPostRequestBody();
$requestBody->setIds(['String', 'String', 'String', ]);

$requestBody->setMemberEntityType('#microsoft.graph.windowsUpdates.azureADDevice');



$graphServiceClient->admin()->windows()->updates()->updatableAssetsById('updatableAsset-id')->windowsUpdatesRemoveMembersById()->post($requestBody);


```