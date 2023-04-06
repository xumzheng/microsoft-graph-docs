---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Team()
request_body.setDisplayName('My Sample Team')

request_body.setDescription('My Sample Team’s Description')

membersConversationMember1 = ConversationMember()
membersConversationMember1.set@odatatype('#microsoft.graph.aadUserConversationMember')

membersConversationMember1.setRoles(['owner', ])

additionalData = [
'user@odata.bind' => 'https://graph.microsoft.com/v1.0/users(\'jacob@contoso.com\')', 
];
membersConversationMember1.setAdditionalData(additionalData)



membersArray []= membersConversationMember1;
request_body.setMembers(membersArray)


additionalData = [
'template@odata.bind' => 'https://graph.microsoft.com/v1.0/teamsTemplates(\'standard\')', 
];
request_body.setAdditionalData(additionalData)



request_config = TeamsRequestBuilderPostRequestConfiguration(
request_config = TeamsRequestBuilderPostRequestConfiguration(query_params=)


result = await client.teams.post(request_body, headers=)


```