---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ChatMessage()
body = ItemBody()
body.setContentType(BodyType('html'))

body.setContent('<div><div><at id=\"0\">TestTag</at>&nbsp;Testing Tags</div></div>')


request_body.setBody($body)
mentionsChatMessageMention1 = ChatMessageMention()
mentionsChatMessageMention1.setId(0)

mentionsChatMessageMention1.setMentionText('TestTag')

mentionsChatMessageMention1Mentioned = ChatMessageMentionedIdentitySet()
mentionsChatMessageMention1MentionedTag = TeamworkTagIdentity()
mentionsChatMessageMention1MentionedTag.setId('MjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyM2OGEzZTM2NS1mN2Q5LTRhNTYtYjQ5OS0yNDMzMmE5Y2M1NzIjI3RTMERJZ1Z1ZQ==')

mentionsChatMessageMention1MentionedTag.setDisplayName('TestTag')


mentionsChatMessageMention1Mentioned.setTag($mentionsChatMessageMention1MentionedTag)

mentionsChatMessageMention1.setMentioned($mentionsChatMessageMention1Mentioned)

mentionsArray []= mentionsChatMessageMention1;
request_body.setMentions(mentionsArray)




result = await client.teams._by_id('team-id').channels._by_id('channel-id').messages.post(request_body)


```