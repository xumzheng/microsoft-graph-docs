---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Channel()
request_body.displayName = 'My First Shared Channel'

request_body.description = 'This is my first shared channel'

request_body.MembershipType(ChannelMembershipType('shared'))

membersConversationMember1 = ConversationMember()
membersConversationMember1.@odatatype = '#microsoft.graph.aadUserConversationMember'

membersConversationMember1.Roles(['owner', ])

additionalData = [
'user@odata.bind' => 'https://graph.microsoft.com/v1.0/users(\'7640023f-fe43-573f-9ff4-84a9efe4acd6\')', 
];
membersConversationMember1.additionaldata(additionalData)



membersArray []= membersConversationMember1;
request_body.members(membersArray)




request_configuration = ChannelsRequestBuilderPostRequestConfiguration(
)


result = await client.teams_by_id('team-id').channels.post(request_body = request_body)


```