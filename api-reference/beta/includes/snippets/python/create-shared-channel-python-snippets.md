---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = Channel();
request_body.setDisplayName('My First Shared Channel');

request_body.setDescription('This is my first shared channel');

request_body.setMembershipType(ChannelMembershipType('shared'));

membersConversationMember1 = ConversationMember();
membersConversationMember1.set@odatatype('#microsoft.graph.aadUserConversationMember');

membersConversationMember1.setRoles(['owner', ]);

additionalData = [
'user@odata.bind' => 'https://graph.microsoft.com/beta/users(\'7640023f-fe43-gv3f-9gg4-84a9efe4acd6\')', 
];
membersConversationMember1.setAdditionalData(additionalData);



membersArray []= membersConversationMember1;
request_body.setMembers(membersArray);




result = await client.teamsById('team-id').channels.post(request_body);


```