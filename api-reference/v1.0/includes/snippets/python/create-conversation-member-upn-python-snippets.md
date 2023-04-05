---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ConversationMember()
request_body.set@odatatype('#microsoft.graph.aadUserConversationMember')

request_body.setVisibleHistoryStartDateTime(DateTime('2019-04-18T23:51:43.255Z'))

request_body.setRoles(['owner', ])

additionalData = [
'user@odata.bind' => 'https://graph.microsoft.com/v1.0/users/jacob@contoso.com', 
];
request_body.setAdditionalData(additionalData)




result = await client.chatsby_id('chat-id')_members.post(request_body)


```