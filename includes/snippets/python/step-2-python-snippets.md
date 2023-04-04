---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = Chat();
request_body.setChatType(ChatType('group'));

membersConversationMember1 = ConversationMember();
membersConversationMember1.set@odatatype('#microsoft.graph.aadUserConversationMember');

membersConversationMember1.setRoles(['owner', ]);

additionalData = [
'user@odata.bind' => 'https://graph.microsoft.com/v1.0/users(\'adams@contoso.com\')', 
];
membersConversationMember1.setAdditionalData(additionalData);



membersArray []= membersConversationMember1;
membersConversationMember2 = ConversationMember();
membersConversationMember2.set@odatatype('#microsoft.graph.aadUserConversationMember');

membersConversationMember2.setRoles(['owner', ]);

additionalData = [
'user@odata.bind' => 'https://graph.microsoft.com/v1.0/users(\'gradyA@contoso.com\')', 
];
membersConversationMember2.setAdditionalData(additionalData);



membersArray []= membersConversationMember2;
membersConversationMember3 = ConversationMember();
membersConversationMember3.set@odatatype('#microsoft.graph.aadUserConversationMember');

membersConversationMember3.setRoles(['owner', ]);

additionalData = [
'user@odata.bind' => 'https://graph.microsoft.com/v1.0/users(\'4562bcc8-c436-4f95-b7c0-4f8ce89dca5e\')', 
];
membersConversationMember3.setAdditionalData(additionalData);



membersArray []= membersConversationMember3;
request_body.setMembers(membersArray);




result = await client.chats.post(request_body);


```