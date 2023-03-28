---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new ConversationMember();
$requestBody.set@odatatype('#microsoft.graph.aadUserConversationMember');

$requestBody.setRoles(['owner', ]);

$additionalData = [
'user@odata.bind' => 'https://graph.microsoft.com/beta/users(\'8b081ef6-4792-4def-b2c9-c363a1bf41d5\')', 
];
$requestBody.setAdditionalData($additionalData);




$requestResult = $graphServiceClient.teamsById('team-id').channelsById('channel-id').members().post($requestBody);


```