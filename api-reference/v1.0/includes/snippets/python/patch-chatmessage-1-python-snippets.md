---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ChatMessage()
request_body.MessageType(ChatMessageType('message'))

request_body.subject=null

request_body.summary=null

request_body.Importance(ChatMessageImportance('normal'))

request_body.locale = 'en-us'

from = ChatMessageFromIdentitySet()
From.application=null

From.device=null

fromUser = Identity()
fromUser.id = '3b102402-813e-4e17-a6b2-f841aef1fdfc'

fromUser.displayName = 'Lam Cong'

additionalData = [
'userIdentityType' => 'aadUser', 
];
fromUser.additionaldata(additionalData)



from.user = fromUser
additionalData = [
'conversation' => 		null,
];
from.additionaldata(additionalData)



request_body.from = from
body = ItemBody()
body.ContentType(BodyType('text'))

body.content = 'Edit text only'


request_body.body = body
request_body.Attachments([])

request_body.Mentions([])

request_body.Reactions([])



request_configuration = ChatMessageRequestBuilderPatchRequestConfiguration(
)


result = await client.teams_by_id('team-id').channels_by_id('channel-id').messages_by_id('chatMessage-id').patch(request_body = request_body)


```