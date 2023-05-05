---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ChatMessage()
request_body.messagetype(ChatMessageType.Message('chatmessagetype.message'))

request_body.subject=null

request_body.summary=null

request_body.importance(ChatMessageImportance.Normal('chatmessageimportance.normal'))

request_body.locale = 'en-us'

from = ChatMessageFromIdentitySet()
from.application=null

from.device=null

fromuser = Identity()
fromuser.id = '3b102402-813e-4e17-a6b2-f841aef1fdfc'

fromuser.display_name = 'Lam Cong'

additional_data = [
'user_identity_type' => 'aadUser', 
];
fromuser.additional_data(additional_data)



from.user = fromuser
additional_data = [
'conversation' => 		null,
];
from.additional_data(additional_data)



request_body.from = from
body = ItemBody()
body.contenttype(BodyType.Html('bodytype.html'))

body.content = '<p><em>text</em></p><attachment id=\"e8f78756199240b88448ae0fc6db112d\"></attachment><attachment id=\"638464e32834471ea202007da60a5ae6\"></attachment>'


request_body.body = body
attachments_chat_message_attachment1 = ChatMessageAttachment()
attachments_chat_message_attachment1.id = 'e8f78756199240b88448ae0fc6db112d'

attachments_chat_message_attachment1.content_type = 'application/vnd.microsoft.card.hero'

attachments_chat_message_attachment1.contentUrl=null

attachments_chat_message_attachment1.content = '{\r\n  \"title\": \"*title*\",\r\n  \"subtitle\": \"*subtitle*\",\r\n  \"text\": \"Have you found yourself scratching your head trying to figure these questions out? Frustrated trying to access some of the goodies unique to the Microsoft Teams platform?  Well, fear not, Bot Builder SDK Extension for Teams in .NET and Node flavors is here!  Just head on over to Nuget or NPM to download our tasty helpers, sure to speed up your prep time so you can spend more time maximizing the flavor of the bots you\'re cooking up.Here’s a small sample of some recipes to whet your appetite.\",\r\n  \"images\": [\r\n    {\r\n      \"url\": \"https://us-api.asm.skype.com/v1/objects/0-eus-d8-ced0c9567ee7b0b233b987bd32f9eacd/views/img_preview\"\r\n    }\r\n  ],\r\n  \"buttons\": [\r\n    {\r\n      \"type\": \"openUrl\",\r\n      \"image\": \"https://urlp.asm.skype.com/v1/url/content?url=https%3a%2f%2fcdn2.iconfinder.com%2fdata%2ficons%2fsocial-icons-33%2f128%2fTrello-128.png\",\r\n      \"title\": \"😃😃 click me 😃😃\",\r\n      \"value\": \"http://microsoft.com\"\r\n    },\r\n    {\r\n      \"type\": \"imback\",\r\n      \"title\": \"&i am back& <>= \\"\",\r\n      \"value\": \"&i am back& <>= \\"\"\r\n    },\r\n    {\r\n      \"type\": \"openUrl\",\r\n      \"title\": \"Open URL\",\r\n      \"value\": \"http://google.com\"\r\n    }\r\n  ]\r\n}'

attachments_chat_message_attachment1.name=null

attachments_chat_message_attachment1.thumbnailUrl=null


attachmentsArray []= attachmentsChatMessageAttachment1;
attachments_chat_message_attachment2 = ChatMessageAttachment()
attachments_chat_message_attachment2.id = '638464e32834471ea202007da60a5ae6'

attachments_chat_message_attachment2.content_type = 'application/vnd.microsoft.card.hero'

attachments_chat_message_attachment2.contentUrl=null

attachments_chat_message_attachment2.content = '{\r\n  \"title\": \"*title*\",\r\n  \"subtitle\": \"*subtitle*\",\r\n  \"text\": \"Have you found yourself scratching your head trying to figure these questions out? Frustrated trying to access some of the goodies unique to the Microsoft Teams platform?  Well, fear not, Bot Builder SDK Extension for Teams in .NET and Node flavors is here!  Just head on over to Nuget or NPM to download our tasty helpers, sure to speed up your prep time so you can spend more time maximizing the flavor of the bots you\'re cooking up.Here’s a small sample of some recipes to whet your appetite.\",\r\n  \"images\": [\r\n    {\r\n      \"url\": \"https://us-api.asm.skype.com/v1/objects/0-eus-d8-ced0c9567ee7b0b233b987bd32f9eacd/views/img_preview\"\r\n    }\r\n  ],\r\n  \"buttons\": [\r\n    {\r\n      \"type\": \"messageBack\",\r\n      \"title\": \"&message back& <>= \\"\",\r\n      \"text\": \"text = &message back& <>= \\"\",\r\n      \"displayText\": \"displayText = &message back& <>= \\"\",\r\n      \"value\": {\r\n        \"text\": \"some text 2\"\r\n      }\r\n    }\r\n  ]\r\n}'

attachments_chat_message_attachment2.name=null

attachments_chat_message_attachment2.thumbnailUrl=null


attachmentsArray []= attachmentsChatMessageAttachment2;
request_body.attachments(attachmentsArray)


request_body.Mentions([])

reactions_chat_message_reaction1 = ChatMessageReaction()
reactions_chat_message_reaction1.reaction_type = 'angry'

reactions_chat_message_reaction1.createdDateTime = DateTime('2018-10-21T08:10:30.489Z')

reactions_chat_message_reaction1user = ChatMessageReactionIdentitySet()
reactions_chat_message_reaction1user.application=null

reactions_chat_message_reaction1user.device=null

reactions_chat_message_reaction1useruser = Identity()
reactions_chat_message_reaction1useruser.id = 'f1b66449-b46d-49b0-9c3c-53c10a5c818e'

reactions_chat_message_reaction1useruser.displayName=null

additional_data = [
'user_identity_type' => 'aadUser', 
];
reactions_chat_message_reaction1useruser.additional_data(additional_data)



reactions_chat_message_reaction1user.user = reactions_chat_message_reaction1useruser

reactions_chat_message_reaction1.user = reactions_chat_message_reaction1user

reactionsArray []= reactionsChatMessageReaction1;
reactions_chat_message_reaction2 = ChatMessageReaction()
reactions_chat_message_reaction2.reaction_type = 'laugh'

reactions_chat_message_reaction2.createdDateTime = DateTime('2018-10-21T08:10:32.489Z')

reactions_chat_message_reaction2user = ChatMessageReactionIdentitySet()
reactions_chat_message_reaction2user.application=null

reactions_chat_message_reaction2user.device=null

reactions_chat_message_reaction2useruser = Identity()
reactions_chat_message_reaction2useruser.id = '03a02232-d8f5-4970-a77e-6e8c76ce7a4e'

reactions_chat_message_reaction2useruser.displayName=null

additional_data = [
'user_identity_type' => 'aadUser', 
];
reactions_chat_message_reaction2useruser.additional_data(additional_data)



reactions_chat_message_reaction2user.user = reactions_chat_message_reaction2useruser

reactions_chat_message_reaction2.user = reactions_chat_message_reaction2user

reactionsArray []= reactionsChatMessageReaction2;
reactions_chat_message_reaction3 = ChatMessageReaction()
reactions_chat_message_reaction3.reaction_type = 'like'

reactions_chat_message_reaction3.createdDateTime = DateTime('2018-10-21T02:17:14.67Z')

reactions_chat_message_reaction3user = ChatMessageReactionIdentitySet()
reactions_chat_message_reaction3user.application=null

reactions_chat_message_reaction3user.device=null

reactions_chat_message_reaction3useruser = Identity()
reactions_chat_message_reaction3useruser.id = 'f1b66449-b46d-49b0-9c3c-53c10a5c818e'

reactions_chat_message_reaction3useruser.displayName=null

additional_data = [
'user_identity_type' => 'aadUser', 
];
reactions_chat_message_reaction3useruser.additional_data(additional_data)



reactions_chat_message_reaction3user.user = reactions_chat_message_reaction3useruser

reactions_chat_message_reaction3.user = reactions_chat_message_reaction3user

reactionsArray []= reactionsChatMessageReaction3;
reactions_chat_message_reaction4 = ChatMessageReaction()
reactions_chat_message_reaction4.reaction_type = 'like'

reactions_chat_message_reaction4.createdDateTime = DateTime('2018-10-21T02:34:40.3Z')

reactions_chat_message_reaction4user = ChatMessageReactionIdentitySet()
reactions_chat_message_reaction4user.application=null

reactions_chat_message_reaction4user.device=null

reactions_chat_message_reaction4useruser = Identity()
reactions_chat_message_reaction4useruser.id = '4c9041b7-449a-40f7-8855-56da239b9fd1'

reactions_chat_message_reaction4useruser.displayName=null

additional_data = [
'user_identity_type' => 'aadUser', 
];
reactions_chat_message_reaction4useruser.additional_data(additional_data)



reactions_chat_message_reaction4user.user = reactions_chat_message_reaction4useruser

reactions_chat_message_reaction4.user = reactions_chat_message_reaction4user

reactionsArray []= reactionsChatMessageReaction4;
reactions_chat_message_reaction5 = ChatMessageReaction()
reactions_chat_message_reaction5.reaction_type = 'like'

reactions_chat_message_reaction5.createdDateTime = DateTime('2018-10-21T08:10:25.489Z')

reactions_chat_message_reaction5user = ChatMessageReactionIdentitySet()
reactions_chat_message_reaction5user.application=null

reactions_chat_message_reaction5user.device=null

reactions_chat_message_reaction5useruser = Identity()
reactions_chat_message_reaction5useruser.id = '03a02232-d8f5-4970-a77e-6e8c76ce7a4e'

reactions_chat_message_reaction5useruser.displayName=null

additional_data = [
'user_identity_type' => 'aadUser', 
];
reactions_chat_message_reaction5useruser.additional_data(additional_data)



reactions_chat_message_reaction5user.user = reactions_chat_message_reaction5useruser

reactions_chat_message_reaction5.user = reactions_chat_message_reaction5user

reactionsArray []= reactionsChatMessageReaction5;
reactions_chat_message_reaction6 = ChatMessageReaction()
reactions_chat_message_reaction6.reaction_type = 'heart'

reactions_chat_message_reaction6.createdDateTime = DateTime('2018-10-21T08:10:31.489Z')

reactions_chat_message_reaction6user = ChatMessageReactionIdentitySet()
reactions_chat_message_reaction6user.application=null

reactions_chat_message_reaction6user.device=null

reactions_chat_message_reaction6useruser = Identity()
reactions_chat_message_reaction6useruser.id = '03a02232-d8f5-4970-a77e-6e8c76ce7a4e'

reactions_chat_message_reaction6useruser.displayName=null

additional_data = [
'user_identity_type' => 'aadUser', 
];
reactions_chat_message_reaction6useruser.additional_data(additional_data)



reactions_chat_message_reaction6user.user = reactions_chat_message_reaction6useruser

reactions_chat_message_reaction6.user = reactions_chat_message_reaction6user

reactionsArray []= reactionsChatMessageReaction6;
reactions_chat_message_reaction7 = ChatMessageReaction()
reactions_chat_message_reaction7.reaction_type = 'sad'

reactions_chat_message_reaction7.createdDateTime = DateTime('2018-10-21T08:10:33.489Z')

reactions_chat_message_reaction7user = ChatMessageReactionIdentitySet()
reactions_chat_message_reaction7user.application=null

reactions_chat_message_reaction7user.device=null

reactions_chat_message_reaction7useruser = Identity()
reactions_chat_message_reaction7useruser.id = '03a02232-d8f5-4970-a77e-6e8c76ce7a4e'

reactions_chat_message_reaction7useruser.displayName=null

additional_data = [
'user_identity_type' => 'aadUser', 
];
reactions_chat_message_reaction7useruser.additional_data(additional_data)



reactions_chat_message_reaction7user.user = reactions_chat_message_reaction7useruser

reactions_chat_message_reaction7.user = reactions_chat_message_reaction7user

reactionsArray []= reactionsChatMessageReaction7;
reactions_chat_message_reaction8 = ChatMessageReaction()
reactions_chat_message_reaction8.reaction_type = 'surprised'

reactions_chat_message_reaction8.createdDateTime = DateTime('2018-10-21T08:10:34.489Z')

reactions_chat_message_reaction8user = ChatMessageReactionIdentitySet()
reactions_chat_message_reaction8user.application=null

reactions_chat_message_reaction8user.device=null

reactions_chat_message_reaction8useruser = Identity()
reactions_chat_message_reaction8useruser.id = '03a02232-d8f5-4970-a77e-6e8c76ce7a4e'

reactions_chat_message_reaction8useruser.displayName=null

additional_data = [
'user_identity_type' => 'aadUser', 
];
reactions_chat_message_reaction8useruser.additional_data(additional_data)



reactions_chat_message_reaction8user.user = reactions_chat_message_reaction8useruser

reactions_chat_message_reaction8.user = reactions_chat_message_reaction8user

reactionsArray []= reactionsChatMessageReaction8;
request_body.reactions(reactionsArray)





result = await client.teams.by_team_id('team-id').channels.by_channel_id('channel-id').messages.by_message_id('chatMessage-id').patch(request_body = request_body)


```