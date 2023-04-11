---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Channel()
request_body.@odatatype = '#Microsoft.Graph.channel'

request_body.MembershipType(ChannelMembershipType('private'))

request_body.displayName = 'My First Private Channel'

request_body.description = 'This is my first private channels'

membersConversationMember1 = ConversationMember()
membersConversationMember1.@odatatype = '#microsoft.graph.aadUserConversationMember'

membersConversationMember1.Roles(['owner', ])

additionalData = [
'user@odata.bind' => 'https://graph.microsoft.com/beta/users(\'jacob@contoso.com\')', 
];
membersConversationMember1.additionaldata(additionalData)



membersArray []= membersConversationMember1;
request_body.members(membersArray)




request_configuration = ChannelsRequestBuilderPostRequestConfiguration(
)


result = await client.teams_by_id('team-id').channels.post(request_body = request_body)


```