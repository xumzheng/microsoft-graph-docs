---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ChatMessage()
request_body.setMessageType(ChatMessageType('message'))

request_body.setSubject(null)

request_body.setSummary(null)

request_body.setImportance(ChatMessageImportance('normal'))

request_body.setLocale('en-us')

from = ChatMessageFromIdentitySet()
From.setApplication(null)

From.setDevice(null)

fromUser = Identity()
fromUser.setId('3b102402-813e-4e17-a6b2-f841aef1fdfc')

fromUser.setDisplayName('Lam Cong')

additionalData = [
'userIdentityType' => 'aadUser', 
];
fromUser.setAdditionalData(additionalData)



from.setUser($fromUser)
additionalData = [
'conversation' => 		null,
];
from.setAdditionalData(additionalData)



request_body.setFrom($from)
body = ItemBody()
body.setContentType(BodyType('text'))

body.setContent('Edit text only')


request_body.setBody($body)
request_body.setAttachments([])

request_body.setMentions([])

request_body.setReactions([])



result = await client.teams_by_id('team-id').channels_by_id('channel-id').messages_by_id('chatMessage-id').patch(request_body, headers=)


```