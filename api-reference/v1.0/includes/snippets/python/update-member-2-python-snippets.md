---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = ConversationMember();
requestBody.set@odatatype('#microsoft.graph.aadUserConversationMember');

requestBody.setRoles(['owner', ]);



result = await client.teamsById('team-id').membersById('conversationMember-id').patch(requestBody);


```