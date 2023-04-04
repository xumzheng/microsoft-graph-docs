---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = Chat();
request_body.setChatType(ChatType('group'));

request_body.setTopic('Group chat title');

membersConversationMember1 = ConversationMember();
membersConversationMember1.set@odatatype('#microsoft.graph.aadUserConversationMember');

membersConversationMember1.setRoles(['owner', ]);

additionalData = [
'user@odata.bind' => 'https://graph.microsoft.com/v1.0/users(\'8c0a1a67-50ce-4114-bb6c-da9c5dbcf6ca\')', 
];
membersConversationMember1.setAdditionalData(additionalData);



membersArray []= membersConversationMember1;
membersConversationMember2 = ConversationMember();
membersConversationMember2.set@odatatype('#microsoft.graph.aadUserConversationMember');

membersConversationMember2.setRoles(['owner', ]);

additionalData = [
'user@odata.bind' => 'https://graph.microsoft.com/v1.0/users(\'82fe7758-5bb3-4f0d-a43f-e555fd399c6f\')', 
];
membersConversationMember2.setAdditionalData(additionalData);



membersArray []= membersConversationMember2;
membersConversationMember3 = ConversationMember();
membersConversationMember3.set@odatatype('#microsoft.graph.aadUserConversationMember');

membersConversationMember3.setRoles(['owner', ]);

additionalData = [
'user@odata.bind' => 'https://graph.microsoft.com/v1.0/users(\'3626a173-f2bc-4883-bcf7-01514c3bfb82\')', 
];
membersConversationMember3.setAdditionalData(additionalData);



membersArray []= membersConversationMember3;
request_body.setMembers(membersArray);




result = await client.chats().post(request_body);


```