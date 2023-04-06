---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ChatMessage()
body = ItemBody()
body.setContentType(BodyType('html'))

body.setContent('<div><div><at id=\"0\">General</at>&nbsp;Hello there!</div></div>')


request_body.setBody($body)
mentionsChatMessageMention1 = ChatMessageMention()
mentionsChatMessageMention1.setId(0)

mentionsChatMessageMention1.setMentionText('General')

mentionsChatMessageMention1Mentioned = ChatMessageMentionedIdentitySet()
mentionsChatMessageMention1MentionedConversation = TeamworkConversationIdentity()
mentionsChatMessageMention1MentionedConversation.setId('19:0b50940236084d258c97b21bd01917b0@thread.skype')

mentionsChatMessageMention1MentionedConversation.setDisplayName('General')

mentionsChatMessageMention1MentionedConversation.setConversationIdentityType(TeamworkConversationIdentityType('channel'))


mentionsChatMessageMention1Mentioned.setConversation($mentionsChatMessageMention1MentionedConversation)

mentionsChatMessageMention1.setMentioned($mentionsChatMessageMention1Mentioned)

mentionsArray []= mentionsChatMessageMention1;
request_body.setMentions(mentionsArray)



request_config = MessagesRequestBuilderPostRequestConfiguration(
request_config = MessagesRequestBuilderPostRequestConfiguration(query_params=)


result = await client.teams_by_id('team-id').channels_by_id('channel-id').messages.post(request_body, headers=)


```