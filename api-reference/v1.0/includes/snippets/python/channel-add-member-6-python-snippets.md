---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ConversationMember()
request_body.@odatatype = '#microsoft.graph.aadUserConversationMember'

request_body.Roles([])

additionalData = [
'user@odata.bind' => 'https://graph.microsoft.com/beta/users(\'jacob@contoso.com\')', 
];
request_body.additionaldata(additionalData)





result = await client.teams_by_id('team-id').channels_by_id('channel-id').members.post(request_body = request_body)


```