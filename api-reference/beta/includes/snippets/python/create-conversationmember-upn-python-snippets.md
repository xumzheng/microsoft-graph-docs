---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = ConversationMember();
requestBody.set@odatatype('#microsoft.graph.aadUserConversationMember');

requestBody.setRoles(['owner', ]);

additionalData = [
'user@odata.bind' => 'https://graph.microsoft.com/v1.0/users(\'jacob@contoso.com\')', 
];
requestBody.setAdditionalData(additionalData);




requestResult = graphServiceClient.teamsById('team-id').members().post(requestBody);


```