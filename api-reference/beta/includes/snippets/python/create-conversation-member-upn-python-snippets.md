---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = ConversationMember();
requestBody.set@odatatype('#microsoft.graph.aadUserConversationMember');

requestBody.setVisibleHistoryStartDateTime(DateTime('2019-04-18T23:51:43.255Z'));

requestBody.setRoles(['owner', ]);

additionalData = [
'user@odata.bind' => 'https://graph.microsoft.com/beta/users/jacob@contoso.com', 
];
requestBody.setAdditionalData(additionalData);




result = awaitclient.chatsById('chat-id').members().post(requestBody);


```