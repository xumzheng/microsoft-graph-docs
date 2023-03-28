---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new ConversationMember();
$requestBody.set@odatatype('#microsoft.graph.aadUserConversationMember');

$requestBody.setRoles(['owner', ]);



$requestResult = $graphServiceClient.teamsById('team-id').membersById('conversationMember-id').patch($requestBody);


```