---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Chat()
request_body.setChatType(ChatType('oneonone'))

membersConversationMember1 = ConversationMember()
membersConversationMember1.set@odatatype('#microsoft.graph.aadUserConversationMember')

membersConversationMember1.setRoles(['owner', ])

additionalData = [
'user@odata.bind' => 'https://graph.microsoft.com/v1.0/users(\'jacob@contoso.com\')', 
];
membersConversationMember1.setAdditionalData(additionalData)



membersArray []= membersConversationMember1;
membersConversationMember2 = ConversationMember()
membersConversationMember2.set@odatatype('#microsoft.graph.aadUserConversationMember')

membersConversationMember2.setRoles(['owner', ])

additionalData = [
'user@odata.bind' => 'https://graph.microsoft.com/v1.0/users(\'alex@contoso.com\')', 
];
membersConversationMember2.setAdditionalData(additionalData)



membersArray []= membersConversationMember2;
request_body.setMembers(membersArray)




result = await client.chats.post(request_body, headers=)


```