---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ChatMessage()
body = ItemBody()
body.ContentType(BodyType('html'))

body.content = 'Hello World <at id=\"0\">Jane Smith</at>'


request_body.body = body
mentions_chat_message_mention1 = ChatMessageMention()
mentionsChatMessageMention1.id = 0

mentionsChatMessageMention1.mentionText = 'Jane Smith'

mentions_chat_message_mention1_mentioned = ChatMessageMentionedIdentitySet()
mentions_chat_message_mention1_mentioned_user = Identity()
mentionsChatMessageMention1MentionedUser.displayName = 'Jane Smith'

mentionsChatMessageMention1MentionedUser.id = 'ef1c916a-3135-4417-ba27-8eb7bd084193'

additionalData = [
'userIdentityType' => 'aadUser', 
];
mentionsChatMessageMention1MentionedUser.additionaldata(additionalData)



mentionsChatMessageMention1Mentioned.user = mentionsChatMessageMention1MentionedUser

mentionsChatMessageMention1.mentioned = mentionsChatMessageMention1Mentioned

mentionsArray []= mentionsChatMessageMention1;
request_body.mentions(mentionsArray)





result = await client.teams_by_id('team-id').channels_by_id('channel-id').messages.post(request_body = request_body)


```