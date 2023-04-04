---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = MarkChatReadForUserPostRequestBody();
user = TeamworkUserIdentity();
user.setId('d864e79f-a516-4d0f-9fee-0eeb4d61fdc2');

additionalData = [
'tenantId' => '2a690434-97d9-4eed-83a6-f5f13600199a', 
];
user.setAdditionalData(additionalData);



request_body.setUser($user);


await client.chatsById('chat-id').markChatReadForUser.post(request_body);


```