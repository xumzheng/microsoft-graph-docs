---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new Chat();
$requestBody.setChatType(new ChatType('oneonone'));

$membersConversationMember1 = new ConversationMember();
$membersConversationMember1.set@odatatype('#microsoft.graph.aadUserConversationMember');

$membersConversationMember1.setRoles(['owner', ]);

$additionalData = [
'user@odata.bind' => 'https://graph.microsoft.com/beta/users(\'jacob@contoso.com\')', 
];
$membersConversationMember1.setAdditionalData($additionalData);



$membersArray []= $membersConversationMember1;
$membersConversationMember2 = new ConversationMember();
$membersConversationMember2.set@odatatype('#microsoft.graph.aadUserConversationMember');

$membersConversationMember2.setRoles(['owner', ]);

$additionalData = [
'user@odata.bind' => 'https://graph.microsoft.com/beta/users(\'alex@contoso.com\')', 
];
$membersConversationMember2.setAdditionalData($additionalData);



$membersArray []= $membersConversationMember2;
$requestBody.setMembers($membersArray);




$requestResult = $graphServiceClient.chats().post($requestBody);


```