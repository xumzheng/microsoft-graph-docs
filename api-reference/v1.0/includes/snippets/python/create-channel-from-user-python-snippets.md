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
'user@odata.bind' => 'https://graph.microsoft.com/v1.0/users(\'62855810-484b-4823-9e01-60667f8b12ae\')', 
];
membersConversationMember1.setAdditionalData(additionalData)



membersArray []= membersConversationMember1;
request_body.setMembers(membersArray)




result = await client.teamsById('team-id').channels.post(request_body)


```