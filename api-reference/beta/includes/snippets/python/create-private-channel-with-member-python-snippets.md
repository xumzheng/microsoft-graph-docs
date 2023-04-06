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
'user@odata.bind' => 'https://graph.microsoft.com/beta/users(\'62855810-484b-4823-9e01-60667f8b12ae\')', 
];
membersConversationMember1.setAdditionalData(additionalData)



membersArray []= membersConversationMember1;
request_body.setMembers(membersArray)



request_config = ChannelsRequestBuilderPostRequestConfiguration(
request_config = ChannelsRequestBuilderPostRequestConfiguration(query_params=)


result = await client.teams_by_id('team-id').channels.post(request_body, headers=)


```