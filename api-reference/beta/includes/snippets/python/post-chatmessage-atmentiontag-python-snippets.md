---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Chat_message()
body = Item_body()
body.contenttype(BodyType.Html('bodytype.html'))

body.content = '<div><div><at id=\"0\">TestTag</at>&nbsp;Testing Tags</div></div>'


request_body.body = body
mentions_chat_message_mention1 = Chat_message_mention()
mentions_chat_message_mention1.Id = 0

mentions_chat_message_mention1.mention_text = 'TestTag'

mentions_chat_message_mention1mentioned = Chat_message_mentioned_identity_set()
mentions_chat_message_mention1mentionedtag = Teamwork_tag_identity()
mentions_chat_message_mention1mentionedtag.id = 'MjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyM2OGEzZTM2NS1mN2Q5LTRhNTYtYjQ5OS0yNDMzMmE5Y2M1NzIjI3RTMERJZ1Z1ZQ=='

mentions_chat_message_mention1mentionedtag.display_name = 'TestTag'


mentions_chat_message_mention1mentioned.tag = mentions_chat_message_mention1mentionedtag

mentions_chat_message_mention1.mentioned = mentions_chat_message_mention1mentioned

mentionsArray []= mentionsChatMessageMention1;
request_body.mentions(mentionsArray)





result = await client.teams.by_team_id('team-id').channels.by_channel_id('channel-id').messages.post(request_body = request_body)


```