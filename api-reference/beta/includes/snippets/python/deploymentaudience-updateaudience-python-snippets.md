---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = UpdateAudiencePostRequestBody()
add_members_updatable_asset1 = UpdatableAsset()
addMembersUpdatableAsset1.@odatatype = '#microsoft.graph.windowsUpdates.azureADDevice'

addMembersUpdatableAsset1.id = 'String (identifier)'


addMembersArray []= addMembersUpdatableAsset1;
request_body.addmembers(addMembersArray)





await client.admin.windows.updates.deploymentAudiences_by_id('deploymentAudience-id').windowsUpdatesupdateAudience.post(request_body = request_body)


```