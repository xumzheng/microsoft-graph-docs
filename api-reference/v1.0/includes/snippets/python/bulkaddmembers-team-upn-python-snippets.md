---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new AddPostRequestBody();
$valuesConversationMember1 = new ConversationMember();
$valuesConversationMember1.set@odatatype('microsoft.graph.aadUserConversationMember');

$valuesConversationMember1.setRoles([]);

$additionalData = [
'user@odata.bind' => 'https://graph.microsoft.com/v1.0/users(\'jacob@contoso.com\')', 
];
$valuesConversationMember1.setAdditionalData($additionalData);



$valuesArray []= $valuesConversationMember1;
$valuesConversationMember2 = new ConversationMember();
$valuesConversationMember2.set@odatatype('microsoft.graph.aadUserConversationMember');

$valuesConversationMember2.setRoles(['owner', ]);

$additionalData = [
'user@odata.bind' => 'https://graph.microsoft.com/v1.0/users(\'alex@contoso.com\')', 
];
$valuesConversationMember2.setAdditionalData($additionalData);



$valuesArray []= $valuesConversationMember2;
$requestBody.setValues($valuesArray);




$requestResult = $graphServiceClient.teamsById('team-id').members().add().post($requestBody);


```