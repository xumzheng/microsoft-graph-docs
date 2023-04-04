---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = Chat();
request_body.setChatType(ChatType('oneonone'));

membersConversationMember1 = ConversationMember();
membersConversationMember1.set@odatatype('#microsoft.graph.aadUserConversationMember');

membersConversationMember1.setRoles(['owner', ]);

additionalData = [
'user@odata.bind' => 'https://graph.microsoft.com/v1.0/users(\'8b081ef6-4792-4def-b2c9-c363a1bf41d5\')', 
];
membersConversationMember1.setAdditionalData(additionalData);



membersArray []= membersConversationMember1;
membersConversationMember2 = ConversationMember();
membersConversationMember2.set@odatatype('#microsoft.graph.aadUserConversationMember');

membersConversationMember2.setRoles(['owner', ]);

additionalData = [
'user@odata.bind' => 'https://graph.microsoft.com/v1.0/users(\'82af01c5-f7cc-4a2e-a728-3a5df21afd9d\')', 
'tenantId' => '4dc1fe35-8ac6-4f0d-904a-7ebcd364bea1', 
];
membersConversationMember2.setAdditionalData(additionalData);



membersArray []= membersConversationMember2;
request_body.setMembers(membersArray);




result = await client.chats().post(request_body);


```