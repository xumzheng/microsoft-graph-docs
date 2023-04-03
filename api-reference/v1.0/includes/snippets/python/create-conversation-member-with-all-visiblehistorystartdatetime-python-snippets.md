---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = ConversationMember();
requestBody.set@odatatype('#microsoft.graph.aadUserConversationMember');

requestBody.setVisibleHistoryStartDateTime(DateTime('0001-01-01T00:00:00Z'));

requestBody.setRoles(['owner', ]);

additionalData = [
'user@odata.bind' => 'https://graph.microsoft.com/v1.0/users/8b081ef6-4792-4def-b2c9-c363a1bf41d5', 
];
requestBody.setAdditionalData(additionalData);




requestResult = graphServiceClient.chatsById('chat-id').members().post(requestBody);


```