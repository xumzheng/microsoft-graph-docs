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
'user@odata.bind' => 'https://graph.microsoft.com/beta/users(\'0040b377-61d8-43db-94f5-81374122dc7e\')', 
];
membersConversationMember1.setAdditionalData(additionalData)



membersArray []= membersConversationMember1;
request_body.setMembers(membersArray)


additionalData = [
'template@odata.bind' => 'https://graph.microsoft.com/beta/teamsTemplates(\'standard\')', 
];
request_body.setAdditionalData(additionalData)



request_config = TeamsRequestBuilderPostRequestConfiguration(
request_config = TeamsRequestBuilderPostRequestConfiguration(query_params=)


result = await client.teams.post(request_body, headers=)


```