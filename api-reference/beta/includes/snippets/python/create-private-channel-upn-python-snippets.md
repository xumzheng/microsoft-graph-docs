---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Channel()
request_body.set@odatatype('#Microsoft.Graph.channel')

request_body.setMembershipType(ChannelMembershipType('private'))

request_body.setDisplayName('My First Private Channel')

request_body.setDescription('This is my first private channels')

membersConversationMember1 = ConversationMember()
membersConversationMember1.set@odatatype('#microsoft.graph.aadUserConversationMember')

membersConversationMember1.setRoles(['owner', ])

additionalData = [
'user@odata.bind' => 'https://graph.microsoft.com/beta/users(\'jacob@contoso.com\')', 
];
membersConversationMember1.setAdditionalData(additionalData)



membersArray []= membersConversationMember1;
request_body.setMembers(membersArray)




result = await client.teamsby_id('team-id')_channels.post(request_body)


```