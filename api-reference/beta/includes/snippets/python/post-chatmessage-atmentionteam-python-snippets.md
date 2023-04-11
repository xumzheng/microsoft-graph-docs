---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ChatMessage()
body = ItemBody()
body.ContentType(BodyType('html'))

body.content = '<div><div><at id=\"0\">GraphTesting</at>&nbsp;Hello team</div></div>'


request_body.body = body
mentionsChatMessageMention1 = ChatMessageMention()
mentionsChatMessageMention1.id = 0

mentionsChatMessageMention1.mentionText = 'GraphTesting'

mentionsChatMessageMention1Mentioned = ChatMessageMentionedIdentitySet()
mentionsChatMessageMention1MentionedConversation = TeamworkConversationIdentity()
mentionsChatMessageMention1MentionedConversation.id = '68a3e365-f7d9-4a56-b499-24332a9cc572'

mentionsChatMessageMention1MentionedConversation.displayName = 'GraphTesting'

mentionsChatMessageMention1MentionedConversation.ConversationIdentityType(TeamworkConversationIdentityType('team'))


mentionsChatMessageMention1Mentioned.conversation = mentionsChatMessageMention1MentionedConversation

mentionsChatMessageMention1.mentioned = mentionsChatMessageMention1Mentioned

mentionsArray []= mentionsChatMessageMention1;
request_body.mentions(mentionsArray)


request_body.Reactions([])

request_body.MessageHistory([])



request_configuration = MessagesRequestBuilderPostRequestConfiguration(
)


result = await client.teams_by_id('team-id').channels_by_id('channel-id').messages.post(request_body = request_body)


```