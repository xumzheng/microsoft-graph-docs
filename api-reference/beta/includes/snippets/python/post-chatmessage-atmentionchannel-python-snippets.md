---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ChatMessage()
body = ItemBody()
body.ContentType(BodyType('html'))

body.content = '<div><div><at id=\"0\">General</at>&nbsp;Hello there!</div></div>'


request_body.body = body
mentions_chat_message_mention1 = ChatMessageMention()
mentionsChatMessageMention1.id = 0

mentionsChatMessageMention1.mentionText = 'General'

mentions_chat_message_mention1_mentioned = ChatMessageMentionedIdentitySet()
mentions_chat_message_mention1_mentioned_conversation = TeamworkConversationIdentity()
mentionsChatMessageMention1MentionedConversation.id = '19:0b50940236084d258c97b21bd01917b0@thread.skype'

mentionsChatMessageMention1MentionedConversation.displayName = 'General'

mentionsChatMessageMention1MentionedConversation.ConversationIdentityType(TeamworkConversationIdentityType('channel'))


mentionsChatMessageMention1Mentioned.conversation = mentionsChatMessageMention1MentionedConversation

mentionsChatMessageMention1.mentioned = mentionsChatMessageMention1Mentioned

mentionsArray []= mentionsChatMessageMention1;
request_body.mentions(mentionsArray)





result = await client.teams_by_id('team-id').channels_by_id('channel-id').messages.post(request_body = request_body)


```