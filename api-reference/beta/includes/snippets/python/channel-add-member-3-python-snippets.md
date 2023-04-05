---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ConversationMember()
request_body.set@odatatype('#microsoft.graph.aadUserConversationMember')

request_body.setRoles(['owner', ])

additionalData = [
'user@odata.bind' => 'https://graph.microsoft.com/beta/users(\'jacob@contoso.com\')', 
];
request_body.setAdditionalData(additionalData)




result = await client.teams._by_id('team-id').channels._by_id('channel-id').members.post(request_body)


```