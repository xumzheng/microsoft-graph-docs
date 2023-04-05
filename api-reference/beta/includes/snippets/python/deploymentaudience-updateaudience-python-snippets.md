---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = UpdateAudiencePostRequestBody()
addMembersUpdatableAsset1 = UpdatableAsset()
addMembersUpdatableAsset1.set@odatatype('#microsoft.graph.windowsUpdates.azureADDevice')

addMembersUpdatableAsset1.setId('String (identifier)')


addMembersArray []= addMembersUpdatableAsset1;
request_body.setAddMembers(addMembersArray)




await client.admin_windows_updates_deploymentAudiencesby_id('deploymentAudience-id')_windowsUpdatesupdateAudience.post(request_body)


```