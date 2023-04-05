---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ChatMessage()
request_body.setMessageType(ChatMessageType('message'))

request_body.setDeletedDateTime(null)

request_body.setSubject(null)

request_body.setSummary(null)

request_body.setImportance(ChatMessageImportance('normal'))

request_body.setLocale('en-us')

from = ChatMessageFromIdentitySet()
From.setApplication(null)

From.setDevice(null)

fromUser = Identity()
fromUser.setId('6b3f3c54-d09c-4fdd-b146-9b514a8a4f40')

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
body.setContentType(BodyType('html'))

body.setContent('<div><div>\n<div>\n<div>\n<div>\n<div><at id=\"0\">Raghav</at><at id=\"1\">TestGlobalBot</at> YEAH')


request_body.setBody($body)
request_body.setAttachments([])

mentionsChatMessageMention1 = ChatMessageMention()
mentionsChatMessageMention1.setId(0)

mentionsChatMessageMention1.setMentionText('Raghav')

mentionsChatMessageMention1Mentioned = ChatMessageMentionedIdentitySet()
mentionsChatMessageMention1Mentioned.setApplication(null)

mentionsChatMessageMention1Mentioned.setDevice(null)

mentionsChatMessageMention1Mentioned.setConversation(null)

mentionsChatMessageMention1MentionedUser = Identity()
mentionsChatMessageMention1MentionedUser.setId('f1b66449-b46d-49b0-9c3c-53c10234c818e')

mentionsChatMessageMention1MentionedUser.setDisplayName('Lam Cong')

additionalData = [
'userIdentityType' => 'aadUser', 
];
mentionsChatMessageMention1MentionedUser.setAdditionalData(additionalData)



mentionsChatMessageMention1Mentioned.setUser($mentionsChatMessageMention1MentionedUser)

mentionsChatMessageMention1.setMentioned($mentionsChatMessageMention1Mentioned)

mentionsArray []= mentionsChatMessageMention1;
mentionsChatMessageMention2 = ChatMessageMention()
mentionsChatMessageMention2.setId(1)

mentionsChatMessageMention2.setMentionText('TestGlobalBot')

mentionsChatMessageMention2Mentioned = ChatMessageMentionedIdentitySet()
mentionsChatMessageMention2MentionedApplication = Identity()
mentionsChatMessageMention2MentionedApplication.setId('03a02232-d8f5-4970-a77e-6e8c76ce7a4e')

mentionsChatMessageMention2MentionedApplication.setDisplayName('TestGlobalBot')

additionalData = [
'applicationIdentityType' => 'bot', 
];
mentionsChatMessageMention2MentionedApplication.setAdditionalData(additionalData)



mentionsChatMessageMention2Mentioned.setApplication($mentionsChatMessageMention2MentionedApplication)
mentionsChatMessageMention2Mentioned.setDevice(null)

mentionsChatMessageMention2Mentioned.setConversation(null)

mentionsChatMessageMention2Mentioned.setUser(null)


mentionsChatMessageMention2.setMentioned($mentionsChatMessageMention2Mentioned)

mentionsArray []= mentionsChatMessageMention2;
request_body.setMentions(mentionsArray)


request_body.setReactions([])



result = await client.teamsby_id('team-id')_channelsby_id('channel-id')_messagesby_id('chatMessage-id').patch(request_body)


```