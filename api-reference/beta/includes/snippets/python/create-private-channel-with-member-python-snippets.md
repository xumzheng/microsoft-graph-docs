---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = Channel();
requestBody.set@odatatype('#Microsoft.Graph.channel');

requestBody.setMembershipType(ChannelMembershipType('private'));

requestBody.setDisplayName('My First Private Channel');

requestBody.setDescription('This is my first private channels');

membersConversationMember1 = ConversationMember();
membersConversationMember1.set@odatatype('#microsoft.graph.aadUserConversationMember');

membersConversationMember1.setRoles(['owner', ]);

additionalData = [
'user@odata.bind' => 'https://graph.microsoft.com/beta/users(\'62855810-484b-4823-9e01-60667f8b12ae\')', 
];
membersConversationMember1.setAdditionalData(additionalData);



membersArray []= membersConversationMember1;
requestBody.setMembers(membersArray);




requestResult = graphServiceClient.teamsById('team-id').channels().post(requestBody);


```