---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Chat()
request_body.ChatType(ChatType('group'))

request_body.topic = 'Group chat title'

membersConversationMember1 = ConversationMember()
membersConversationMember1.@odatatype = '#microsoft.graph.aadUserConversationMember'

membersConversationMember1.Roles(['owner', ])

additionalData = [
'user@odata.bind' => 'https://graph.microsoft.com/beta/users(\'8c0a1a67-50ce-4114-bb6c-da9c5dbcf6ca\')', 
];
membersConversationMember1.additionaldata(additionalData)



membersArray []= membersConversationMember1;
membersConversationMember2 = ConversationMember()
membersConversationMember2.@odatatype = '#microsoft.graph.aadUserConversationMember'

membersConversationMember2.Roles(['owner', ])

additionalData = [
'user@odata.bind' => 'https://graph.microsoft.com/beta/users(\'82fe7758-5bb3-4f0d-a43f-e555fd399c6f\')', 
];
membersConversationMember2.additionaldata(additionalData)



membersArray []= membersConversationMember2;
membersConversationMember3 = ConversationMember()
membersConversationMember3.@odatatype = '#microsoft.graph.aadUserConversationMember'

membersConversationMember3.Roles(['guest', ])

additionalData = [
'user@odata.bind' => 'https://graph.microsoft.com/beta/users(\'8ba98gf6-7fc2-4eb2-c7f2-aef9f21fd98g\')', 
];
membersConversationMember3.additionaldata(additionalData)



membersArray []= membersConversationMember3;
request_body.members(membersArray)




request_configuration = ChatsRequestBuilderPostRequestConfiguration(
)


result = await client.chats.post(request_body = request_body)


```