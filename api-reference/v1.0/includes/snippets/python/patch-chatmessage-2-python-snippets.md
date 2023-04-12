---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ChatMessage()
request_body.MessageType(ChatMessageType('message'))

request_body.deletedDateTime=null

request_body.subject=null

request_body.summary=null

request_body.Importance(ChatMessageImportance('normal'))

request_body.locale = 'en-us'

from = ChatMessageFromIdentitySet()
From.application=null

From.device=null

fromUser = Identity()
fromUser.id = '6b3f3c54-d09c-4fdd-b146-9b514a8a4f40'

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
body.ContentType(BodyType('html'))

body.content = '<div><div>\n<div>\n<div>\n<div>\n<div><at id=\"0\">Raghav</at><at id=\"1\">TestGlobalBot</at> YEAH'


request_body.body = body
request_body.Attachments([])

mentionsChatMessageMention1 = ChatMessageMention()
mentionsChatMessageMention1.id = 0

mentionsChatMessageMention1.mentionText = 'Raghav'

mentionsChatMessageMention1Mentioned = ChatMessageMentionedIdentitySet()
mentionsChatMessageMention1Mentioned.application=null

mentionsChatMessageMention1Mentioned.device=null

mentionsChatMessageMention1Mentioned.conversation=null

mentionsChatMessageMention1MentionedUser = Identity()
mentionsChatMessageMention1MentionedUser.id = 'f1b66449-b46d-49b0-9c3c-53c10234c818e'

mentionsChatMessageMention1MentionedUser.displayName = 'Lam Cong'

additionalData = [
'userIdentityType' => 'aadUser', 
];
mentionsChatMessageMention1MentionedUser.additionaldata(additionalData)



mentionsChatMessageMention1Mentioned.user = mentionsChatMessageMention1MentionedUser

mentionsChatMessageMention1.mentioned = mentionsChatMessageMention1Mentioned

mentionsArray []= mentionsChatMessageMention1;
mentionsChatMessageMention2 = ChatMessageMention()
mentionsChatMessageMention2.id = 1

mentionsChatMessageMention2.mentionText = 'TestGlobalBot'

mentionsChatMessageMention2Mentioned = ChatMessageMentionedIdentitySet()
mentionsChatMessageMention2MentionedApplication = Identity()
mentionsChatMessageMention2MentionedApplication.id = '03a02232-d8f5-4970-a77e-6e8c76ce7a4e'

mentionsChatMessageMention2MentionedApplication.displayName = 'TestGlobalBot'

additionalData = [
'applicationIdentityType' => 'bot', 
];
mentionsChatMessageMention2MentionedApplication.additionaldata(additionalData)



mentionsChatMessageMention2Mentioned.application = mentionsChatMessageMention2MentionedApplication
mentionsChatMessageMention2Mentioned.device=null

mentionsChatMessageMention2Mentioned.conversation=null

mentionsChatMessageMention2Mentioned.user=null


mentionsChatMessageMention2.mentioned = mentionsChatMessageMention2Mentioned

mentionsArray []= mentionsChatMessageMention2;
request_body.mentions(mentionsArray)


request_body.Reactions([])




result = await client.teams_by_id('team-id').channels_by_id('channel-id').messages_by_id('chatMessage-id').patch(request_body = request_body)


```