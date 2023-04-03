---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = ConversationMember();
requestBody.set@odatatype('#microsoft.graph.aadUserConversationMember');

requestBody.setRoles([]);

additionalData = [
'user@odata.bind' => 'https://graph.microsoft.com/beta/users(\'jacob@contoso.com\')', 
];
requestBody.setAdditionalData(additionalData);




result = await client.teamsById('team-id').channelsById('channel-id').members().post(requestBody);


```