---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = Channel();
requestBody.setDisplayName('My First Shared Channel');

requestBody.setDescription('This is my first shared channel');

requestBody.setMembershipType(ChannelMembershipType('shared'));

membersConversationMember1 = ConversationMember();
membersConversationMember1.set@odatatype('#microsoft.graph.aadUserConversationMember');

membersConversationMember1.setRoles(['owner', ]);

additionalData = [
'user@odata.bind' => 'https://graph.microsoft.com/beta/users(\'7640023f-fe43-gv3f-9gg4-84a9efe4acd6\')', 
];
membersConversationMember1.setAdditionalData(additionalData);



membersArray []= membersConversationMember1;
requestBody.setMembers(membersArray);




result = await client.teamsById('team-id').channels().post(requestBody);


```