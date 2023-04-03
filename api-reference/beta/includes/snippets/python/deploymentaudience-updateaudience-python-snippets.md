---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = UpdateAudiencePostRequestBody();
addMembersUpdatableAsset1 = UpdatableAsset();
addMembersUpdatableAsset1.set@odatatype('#microsoft.graph.windowsUpdates.azureADDevice');

addMembersUpdatableAsset1.setId('String (identifier)');


addMembersArray []= addMembersUpdatableAsset1;
requestBody.setAddMembers(addMembersArray);




awaitclient.admin().windows().updates().deploymentAudiencesById('deploymentAudience-id').windowsUpdatesUpdateAudience().post(requestBody);


```