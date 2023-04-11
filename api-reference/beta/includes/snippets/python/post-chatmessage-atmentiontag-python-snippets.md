---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ChatMessage()
body = ItemBody()
body.ContentType(BodyType('html'))

body.content = '<div><div><at id=\"0\">TestTag</at>&nbsp;Testing Tags</div></div>'


request_body.body = body
mentionsChatMessageMention1 = ChatMessageMention()
mentionsChatMessageMention1.id = 0

mentionsChatMessageMention1.mentionText = 'TestTag'

mentionsChatMessageMention1Mentioned = ChatMessageMentionedIdentitySet()
mentionsChatMessageMention1MentionedTag = TeamworkTagIdentity()
mentionsChatMessageMention1MentionedTag.id = 'MjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyM2OGEzZTM2NS1mN2Q5LTRhNTYtYjQ5OS0yNDMzMmE5Y2M1NzIjI3RTMERJZ1Z1ZQ=='

mentionsChatMessageMention1MentionedTag.displayName = 'TestTag'


mentionsChatMessageMention1Mentioned.tag = mentionsChatMessageMention1MentionedTag

mentionsChatMessageMention1.mentioned = mentionsChatMessageMention1Mentioned

mentionsArray []= mentionsChatMessageMention1;
request_body.mentions(mentionsArray)




request_configuration = MessagesRequestBuilderPostRequestConfiguration(
)


result = await client.teams_by_id('team-id').channels_by_id('channel-id').messages.post(request_body = request_body)


```