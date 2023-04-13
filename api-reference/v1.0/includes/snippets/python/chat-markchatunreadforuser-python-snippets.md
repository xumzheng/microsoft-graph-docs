---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = MarkChatUnreadForUserPostRequestBody()
user = TeamworkUserIdentity()
user.id = 'd864e79f-a516-4d0f-9fee-0eeb4d61fdc2'

additionalData = [
'tenantId' => '2a690434-97d9-4eed-83a6-f5f13600199a', 
];
user.additionaldata(additionalData)



request_body.user = user
request_body.lastMessageReadDateTime = DateTime('2021-05-27T22:13:01.577Z')




await client.chats_by_id('chat-id').markChatUnreadForUser.post(request_body = request_body)


```