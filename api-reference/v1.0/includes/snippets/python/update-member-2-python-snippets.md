---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ConversationMember()
request_body.set@odatatype('#microsoft.graph.aadUserConversationMember')

request_body.setRoles(['owner', ])


request_config = ConversationMemberRequestBuilderPatchRequestConfiguration(
request_config = ConversationMemberRequestBuilderPatchRequestConfiguration(query_params=)


result = await client.teams_by_id('team-id').members_by_id('conversationMember-id').patch(request_body, headers=)


```