---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = ConversationMember();
requestBody.set@odatatype('#microsoft.graph.aadUserConversationMember');

requestBody.setRoles([]);

additionalData = [
'user@odata.bind' => 'https://graph.microsoft.com/v1.0/users/24b3819b-4e1d-4f3e-86bd-e42b54d0b2b4', 
];
requestBody.setAdditionalData(additionalData);




result = awaitclient.teamsById('team-id').channelsById('channel-id').members().post(requestBody);


```