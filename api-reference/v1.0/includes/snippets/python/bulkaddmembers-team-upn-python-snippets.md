---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AddPostRequestBody()
valuesConversationMember1 = ConversationMember()
valuesConversationMember1.set@odatatype('microsoft.graph.aadUserConversationMember')

valuesConversationMember1.setRoles([])

additionalData = [
'user@odata.bind' => 'https://graph.microsoft.com/v1.0/users(\'jacob@contoso.com\')', 
];
valuesConversationMember1.setAdditionalData(additionalData)



valuesArray []= valuesConversationMember1;
valuesConversationMember2 = ConversationMember()
valuesConversationMember2.set@odatatype('microsoft.graph.aadUserConversationMember')

valuesConversationMember2.setRoles(['owner', ])

additionalData = [
'user@odata.bind' => 'https://graph.microsoft.com/v1.0/users(\'alex@contoso.com\')', 
];
valuesConversationMember2.setAdditionalData(additionalData)



valuesArray []= valuesConversationMember2;
request_body.setValues(valuesArray)




result = await client.teams_by_id('team-id').members.add.post(request_body, headers=)


```