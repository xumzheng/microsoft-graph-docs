---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AddPostRequestBody()
valuesConversationMember1 = ConversationMember()
valuesConversationMember1.@odatatype = 'microsoft.graph.aadUserConversationMember'

valuesConversationMember1.Roles([])

additionalData = [
'user@odata.bind' => 'https://graph.microsoft.com/beta/users(\'jacob@contoso.com\')', 
];
valuesConversationMember1.additionaldata(additionalData)



valuesArray []= valuesConversationMember1;
valuesConversationMember2 = ConversationMember()
valuesConversationMember2.@odatatype = 'microsoft.graph.aadUserConversationMember'

valuesConversationMember2.Roles(['owner', ])

additionalData = [
'user@odata.bind' => 'https://graph.microsoft.com/beta/users(\'alex@contoso.com\')', 
];
valuesConversationMember2.additionaldata(additionalData)



valuesArray []= valuesConversationMember2;
request_body.values(valuesArray)




request_configuration = AddRequestBuilderPostRequestConfiguration(
)


result = await client.teams_by_id('team-id').members.add.post(request_body = request_body)


```