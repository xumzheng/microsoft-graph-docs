---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AddPostRequestBody()
values_conversation_member1 = ConversationMember()
valuesConversationMember1.@odatatype = 'microsoft.graph.aadUserConversationMember'

valuesConversationMember1.Roles([])

additionalData = [
'user@odata.bind' => 'https://graph.microsoft.com/v1.0/users(\'18a80140-b0fb-4489-b360-2f6efaf225a0\')', 
];
valuesConversationMember1.additionaldata(additionalData)



valuesArray []= valuesConversationMember1;
values_conversation_member2 = ConversationMember()
valuesConversationMember2.@odatatype = 'microsoft.graph.aadUserConversationMember'

valuesConversationMember2.Roles(['owner', ])

additionalData = [
'user@odata.bind' => 'https://graph.microsoft.com/v1.0/users(\'86503198-b81b-43fe-81ee-ad45b8848ac9\')', 
];
valuesConversationMember2.additionaldata(additionalData)



valuesArray []= valuesConversationMember2;
request_body.values(valuesArray)





result = await client.teams_by_id('team-id').members.add.post(request_body = request_body)


```