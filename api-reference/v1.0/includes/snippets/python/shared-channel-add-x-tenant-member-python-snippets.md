---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ConversationMember()
request_body.set@odatatype('#microsoft.graph.aadUserConversationMember')

request_body.setRoles([])

additionalData = [
'user@odata.bind' => 'https://graph.microsoft.com/v1.0/users/bc3598dd-cce4-4742-ae15-173429951408', 
'tenantId' => 'a18103d1-a6ef-4f66-ac64-e4ef42ea8681', 
];
request_body.setAdditionalData(additionalData)




result = await client.teams_by_id('team-id').channels_by_id('channel-id').members.post(request_body, headers=)


```