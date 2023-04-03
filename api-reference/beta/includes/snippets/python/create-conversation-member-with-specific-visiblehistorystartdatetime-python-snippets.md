---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = ConversationMember();
requestBody.set@odatatype('#microsoft.graph.aadUserConversationMember');

requestBody.setVisibleHistoryStartDateTime(DateTime('2019-04-18T23:51:43.255Z'));

requestBody.setRoles(['owner', ]);

additionalData = [
'user@odata.bind' => 'https://graph.microsoft.com/beta/users/8b081ef6-4792-4def-b2c9-c363a1bf41d5', 
];
requestBody.setAdditionalData(additionalData);




result = await client.chatsById('chat-id').members().post(requestBody);


```