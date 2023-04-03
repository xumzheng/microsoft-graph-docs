---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = OnPremisesAgentGroup();
requestBody.setDisplayName('Group New Name');



result = awaitclient.onPremisesPublishingProfilesById('onPremisesPublishingProfile-id').agentGroupsById('onPremisesAgentGroup-id').patch(requestBody);


```