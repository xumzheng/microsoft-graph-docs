---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ChatMessage()
body = ItemBody()
body.setContentType(BodyType('html'))

body.setContent('Hello World <at id=\"0\">Jane Smith</at>')


request_body.setBody($body)
mentionsChatMessageMention1 = ChatMessageMention()
mentionsChatMessageMention1.setId(0)

mentionsChatMessageMention1.setMentionText('Jane Smith')

mentionsChatMessageMention1Mentioned = ChatMessageMentionedIdentitySet()
mentionsChatMessageMention1MentionedUser = Identity()
mentionsChatMessageMention1MentionedUser.setDisplayName('Jane Smith')

mentionsChatMessageMention1MentionedUser.setId('ef1c916a-3135-4417-ba27-8eb7bd084193')

additionalData = [
'userIdentityType' => 'aadUser', 
];
mentionsChatMessageMention1MentionedUser.setAdditionalData(additionalData)



mentionsChatMessageMention1Mentioned.setUser($mentionsChatMessageMention1MentionedUser)

mentionsChatMessageMention1.setMentioned($mentionsChatMessageMention1Mentioned)

mentionsArray []= mentionsChatMessageMention1;
request_body.setMentions(mentionsArray)




result = await client.teams_by_id('team-id').channels_by_id('channel-id').messages.post(request_body)


```