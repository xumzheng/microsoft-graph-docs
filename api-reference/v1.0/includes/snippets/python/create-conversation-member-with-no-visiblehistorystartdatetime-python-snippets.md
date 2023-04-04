---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = ConversationMember();
request_body.set@odatatype('#microsoft.graph.aadUserConversationMember');

request_body.setRoles(['owner', ]);

additionalData = [
'user@odata.bind' => 'https://graph.microsoft.com/v1.0/users/8b081ef6-4792-4def-b2c9-c363a1bf41d5', 
];
request_body.setAdditionalData(additionalData);




result = await client.chatsById('chat-id').members.post(request_body);


```