---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = AddPostRequestBody();
valuesConversationMember1 = ConversationMember();
valuesConversationMember1.set@odatatype('microsoft.graph.aadUserConversationMember');

valuesConversationMember1.setRoles([]);

additionalData = [
'user@odata.bind' => 'https://graph.microsoft.com/beta/users(\'18a80140-b0fb-4489-b360-2f6efaf225a0\')', 
];
valuesConversationMember1.setAdditionalData(additionalData);



valuesArray []= valuesConversationMember1;
valuesConversationMember2 = ConversationMember();
valuesConversationMember2.set@odatatype('microsoft.graph.aadUserConversationMember');

valuesConversationMember2.setRoles(['owner', ]);

additionalData = [
'user@odata.bind' => 'https://graph.microsoft.com/beta/users(\'86503198-b81b-43fe-81ee-ad45b8848ac9\')', 
];
valuesConversationMember2.setAdditionalData(additionalData);



valuesArray []= valuesConversationMember2;
requestBody.setValues(valuesArray);




requestResult = graphServiceClient.teamsById('team-id').members().add().post(requestBody);


```