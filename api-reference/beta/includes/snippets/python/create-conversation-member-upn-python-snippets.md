---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new ConversationMember();
$requestBody->set@odatatype('#microsoft.graph.aadUserConversationMember');

$requestBody->setVisibleHistoryStartDateTime(new DateTime('2019-04-18T23:51:43.255Z'));

$requestBody->setRoles(['owner', ]);

$additionalData = [
'user@odata.bind' => 'https://graph.microsoft.com/beta/users/jacob@contoso.com', 
];
$requestBody->setAdditionalData($additionalData);




$requestResult = $graphServiceClient->chatsById('chat-id')->members()->post($requestBody);


```