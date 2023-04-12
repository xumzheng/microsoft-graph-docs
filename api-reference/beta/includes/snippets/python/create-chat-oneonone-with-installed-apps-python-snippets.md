---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Chat()
request_body.ChatType(ChatType('oneonone'))

membersConversationMember1 = ConversationMember()
membersConversationMember1.@odatatype = '#microsoft.graph.aadUserConversationMember'

membersConversationMember1.Roles(['owner', ])

additionalData = [
'user@odata.bind' => 'https://graph.microsoft.com/beta/users(\'8b081ef6-4792-4def-b2c9-c363a1bf41d5\')', 
];
membersConversationMember1.additionaldata(additionalData)



membersArray []= membersConversationMember1;
membersConversationMember2 = ConversationMember()
membersConversationMember2.@odatatype = '#microsoft.graph.aadUserConversationMember'

membersConversationMember2.Roles(['owner', ])

additionalData = [
'user@odata.bind' => 'https://graph.microsoft.com/beta/users(\'82af01c5-f7cc-4a2e-a728-3a5df21afd9d\')', 
];
membersConversationMember2.additionaldata(additionalData)



membersArray []= membersConversationMember2;
request_body.members(membersArray)


installedAppsTeamsAppInstallation1 = TeamsAppInstallation()
additionalData = [
'teamsApp@odata.bind' => 'https://graph.microsoft.com/beta/appCatalogs/teamsApps/05F59CEC-A742-4A50-A62E-202A57E478A4', 
];
installedAppsTeamsAppInstallation1.additionaldata(additionalData)



installedAppsArray []= installedAppsTeamsAppInstallation1;
request_body.installedapps(installedAppsArray)





result = await client.chats.post(request_body = request_body)


```