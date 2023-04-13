---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Team()
request_body.displayName = 'My Sample Team'

request_body.description = 'My Sample Team’s Description'

members_conversation_member1 = ConversationMember()
membersConversationMember1.@odatatype = '#microsoft.graph.aadUserConversationMember'

membersConversationMember1.Roles(['owner', ])

additionalData = [
'user@odata.bind' => 'https://graph.microsoft.com/beta/users(\'jacob@contoso.com\')', 
];
membersConversationMember1.additionaldata(additionalData)



membersArray []= membersConversationMember1;
request_body.members(membersArray)


additionalData = [
'template@odata.bind' => 'https://graph.microsoft.com/beta/teamsTemplates(\'standard\')', 
];
request_body.additionaldata(additionalData)





result = await client.teams.post(request_body = request_body)


```