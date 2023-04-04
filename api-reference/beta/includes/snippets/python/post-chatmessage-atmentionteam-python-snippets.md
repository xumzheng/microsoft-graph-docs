---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = ChatMessage();
body = ItemBody();
body.setContentType(BodyType('html'));

body.setContent('<div><div><at id=\"0\">GraphTesting</at>&nbsp;Hello team</div></div>');


request_body.setBody($body);
mentionsChatMessageMention1 = ChatMessageMention();
mentionsChatMessageMention1.setId(0);

mentionsChatMessageMention1.setMentionText('GraphTesting');

mentionsChatMessageMention1Mentioned = ChatMessageMentionedIdentitySet();
mentionsChatMessageMention1MentionedConversation = TeamworkConversationIdentity();
mentionsChatMessageMention1MentionedConversation.setId('68a3e365-f7d9-4a56-b499-24332a9cc572');

mentionsChatMessageMention1MentionedConversation.setDisplayName('GraphTesting');

mentionsChatMessageMention1MentionedConversation.setConversationIdentityType(TeamworkConversationIdentityType('team'));


mentionsChatMessageMention1Mentioned.setConversation($mentionsChatMessageMention1MentionedConversation);

mentionsChatMessageMention1.setMentioned($mentionsChatMessageMention1Mentioned);

mentionsArray []= mentionsChatMessageMention1;
request_body.setMentions(mentionsArray);


request_body.setReactions([]);

request_body.setMessageHistory([]);



result = await client.teamsById('team-id').channelsById('channel-id').messages.post(request_body);


```