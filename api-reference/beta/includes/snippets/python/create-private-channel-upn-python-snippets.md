---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new Channel();
$requestBody.set@odatatype('#Microsoft.Graph.channel');

$requestBody.setMembershipType(new ChannelMembershipType('private'));

$requestBody.setDisplayName('My First Private Channel');

$requestBody.setDescription('This is my first private channels');

$membersConversationMember1 = new ConversationMember();
$membersConversationMember1.set@odatatype('#microsoft.graph.aadUserConversationMember');

$membersConversationMember1.setRoles(['owner', ]);

$additionalData = [
'user@odata.bind' => 'https://graph.microsoft.com/beta/users(\'jacob@contoso.com\')', 
];
$membersConversationMember1.setAdditionalData($additionalData);



$membersArray []= $membersConversationMember1;
$requestBody.setMembers($membersArray);




$requestResult = $graphServiceClient.teamsById('team-id').channels().post($requestBody);


```