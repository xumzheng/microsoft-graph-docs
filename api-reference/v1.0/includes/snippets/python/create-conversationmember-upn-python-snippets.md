---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ConversationMember()
request_body.@odatatype = '#microsoft.graph.aadUserConversationMember'

request_body.Roles(['owner', ])

additionalData = [
'user@odata.bind' => 'https://graph.microsoft.com/v1.0/users(\'jacob@contoso.com\')', 
];
request_body.additionaldata(additionalData)




request_configuration = MembersRequestBuilderPostRequestConfiguration(
)


result = await client.teams_by_id('team-id').members.post(request_body = request_body)


```