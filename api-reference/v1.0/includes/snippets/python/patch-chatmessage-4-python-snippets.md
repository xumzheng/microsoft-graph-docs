---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ChatMessage()
request_body.MessageType(ChatMessageType('message'))

request_body.subject=null

request_body.summary=null

request_body.Importance(ChatMessageImportance('normal'))

request_body.locale = 'en-us'

from = ChatMessageFromIdentitySet()
From.application=null

From.device=null

fromUser = Identity()
fromUser.id = '3b102402-813e-4e17-a6b2-f841aef1fdfc'

fromUser.displayName = 'Lam Cong'

additionalData = [
'userIdentityType' => 'aadUser', 
];
fromUser.additionaldata(additionalData)



from.user = fromUser
additionalData = [
'conversation' => 		null,
];
from.additionaldata(additionalData)



request_body.from = from
body = ItemBody()
body.ContentType(BodyType('html'))

body.content = '<p><em>text</em></p><attachment id=\"e8f78756199240b88448ae0fc6db112d\"></attachment><attachment id=\"638464e32834471ea202007da60a5ae6\"></attachment>'


request_body.body = body
attachmentsChatMessageAttachment1 = ChatMessageAttachment()
attachmentsChatMessageAttachment1.id = 'e8f78756199240b88448ae0fc6db112d'

attachmentsChatMessageAttachment1.contentType = 'application/vnd.microsoft.card.hero'

attachmentsChatMessageAttachment1.contentUrl=null

attachmentsChatMessageAttachment1.content = '{\r\n  \"title\": \"*title*\",\r\n  \"subtitle\": \"*subtitle*\",\r\n  \"text\": \"Have you found yourself scratching your head trying to figure these questions out? Frustrated trying to access some of the goodies unique to the Microsoft Teams platform?  Well, fear not, Bot Builder SDK Extension for Teams in .NET and Node flavors is here!  Just head on over to Nuget or NPM to download our tasty helpers, sure to speed up your prep time so you can spend more time maximizing the flavor of the bots you\'re cooking up.Here’s a small sample of some recipes to whet your appetite.\",\r\n  \"images\": [\r\n    {\r\n      \"url\": \"https://us-api.asm.skype.com/v1/objects/0-eus-d8-ced0c9567ee7b0b233b987bd32f9eacd/views/img_preview\"\r\n    }\r\n  ],\r\n  \"buttons\": [\r\n    {\r\n      \"type\": \"openUrl\",\r\n      \"image\": \"https://urlp.asm.skype.com/v1/url/content?url=https%3a%2f%2fcdn2.iconfinder.com%2fdata%2ficons%2fsocial-icons-33%2f128%2fTrello-128.png\",\r\n      \"title\": \"😃😃 click me 😃😃\",\r\n      \"value\": \"http://microsoft.com\"\r\n    },\r\n    {\r\n      \"type\": \"imback\",\r\n      \"title\": \"&i am back& <>= \\"\",\r\n      \"value\": \"&i am back& <>= \\"\"\r\n    },\r\n    {\r\n      \"type\": \"openUrl\",\r\n      \"title\": \"Open URL\",\r\n      \"value\": \"http://google.com\"\r\n    }\r\n  ]\r\n}'

attachmentsChatMessageAttachment1.name=null

attachmentsChatMessageAttachment1.thumbnailUrl=null


attachmentsArray []= attachmentsChatMessageAttachment1;
attachmentsChatMessageAttachment2 = ChatMessageAttachment()
attachmentsChatMessageAttachment2.id = '638464e32834471ea202007da60a5ae6'

attachmentsChatMessageAttachment2.contentType = 'application/vnd.microsoft.card.hero'

attachmentsChatMessageAttachment2.contentUrl=null

attachmentsChatMessageAttachment2.content = '{\r\n  \"title\": \"*title*\",\r\n  \"subtitle\": \"*subtitle*\",\r\n  \"text\": \"Have you found yourself scratching your head trying to figure these questions out? Frustrated trying to access some of the goodies unique to the Microsoft Teams platform?  Well, fear not, Bot Builder SDK Extension for Teams in .NET and Node flavors is here!  Just head on over to Nuget or NPM to download our tasty helpers, sure to speed up your prep time so you can spend more time maximizing the flavor of the bots you\'re cooking up.Here’s a small sample of some recipes to whet your appetite.\",\r\n  \"images\": [\r\n    {\r\n      \"url\": \"https://us-api.asm.skype.com/v1/objects/0-eus-d8-ced0c9567ee7b0b233b987bd32f9eacd/views/img_preview\"\r\n    }\r\n  ],\r\n  \"buttons\": [\r\n    {\r\n      \"type\": \"messageBack\",\r\n      \"title\": \"&message back& <>= \\"\",\r\n      \"text\": \"text = &message back& <>= \\"\",\r\n      \"displayText\": \"displayText = &message back& <>= \\"\",\r\n      \"value\": {\r\n        \"text\": \"some text 2\"\r\n      }\r\n    }\r\n  ]\r\n}'

attachmentsChatMessageAttachment2.name=null

attachmentsChatMessageAttachment2.thumbnailUrl=null


attachmentsArray []= attachmentsChatMessageAttachment2;
request_body.attachments(attachmentsArray)


request_body.Mentions([])

reactionsChatMessageReaction1 = ChatMessageReaction()
reactionsChatMessageReaction1.reactionType = 'angry'

reactionsChatMessageReaction1.createdDateTime = DateTime('2018-10-21T08:10:30.489Z')

reactionsChatMessageReaction1User = ChatMessageReactionIdentitySet()
reactionsChatMessageReaction1User.application=null

reactionsChatMessageReaction1User.device=null

reactionsChatMessageReaction1UserUser = Identity()
reactionsChatMessageReaction1UserUser.id = 'f1b66449-b46d-49b0-9c3c-53c10a5c818e'

reactionsChatMessageReaction1UserUser.displayName=null

additionalData = [
'userIdentityType' => 'aadUser', 
];
reactionsChatMessageReaction1UserUser.additionaldata(additionalData)



reactionsChatMessageReaction1User.user = reactionsChatMessageReaction1UserUser

reactionsChatMessageReaction1.user = reactionsChatMessageReaction1User

reactionsArray []= reactionsChatMessageReaction1;
reactionsChatMessageReaction2 = ChatMessageReaction()
reactionsChatMessageReaction2.reactionType = 'laugh'

reactionsChatMessageReaction2.createdDateTime = DateTime('2018-10-21T08:10:32.489Z')

reactionsChatMessageReaction2User = ChatMessageReactionIdentitySet()
reactionsChatMessageReaction2User.application=null

reactionsChatMessageReaction2User.device=null

reactionsChatMessageReaction2UserUser = Identity()
reactionsChatMessageReaction2UserUser.id = '03a02232-d8f5-4970-a77e-6e8c76ce7a4e'

reactionsChatMessageReaction2UserUser.displayName=null

additionalData = [
'userIdentityType' => 'aadUser', 
];
reactionsChatMessageReaction2UserUser.additionaldata(additionalData)



reactionsChatMessageReaction2User.user = reactionsChatMessageReaction2UserUser

reactionsChatMessageReaction2.user = reactionsChatMessageReaction2User

reactionsArray []= reactionsChatMessageReaction2;
reactionsChatMessageReaction3 = ChatMessageReaction()
reactionsChatMessageReaction3.reactionType = 'like'

reactionsChatMessageReaction3.createdDateTime = DateTime('2018-10-21T02:17:14.67Z')

reactionsChatMessageReaction3User = ChatMessageReactionIdentitySet()
reactionsChatMessageReaction3User.application=null

reactionsChatMessageReaction3User.device=null

reactionsChatMessageReaction3UserUser = Identity()
reactionsChatMessageReaction3UserUser.id = 'f1b66449-b46d-49b0-9c3c-53c10a5c818e'

reactionsChatMessageReaction3UserUser.displayName=null

additionalData = [
'userIdentityType' => 'aadUser', 
];
reactionsChatMessageReaction3UserUser.additionaldata(additionalData)



reactionsChatMessageReaction3User.user = reactionsChatMessageReaction3UserUser

reactionsChatMessageReaction3.user = reactionsChatMessageReaction3User

reactionsArray []= reactionsChatMessageReaction3;
reactionsChatMessageReaction4 = ChatMessageReaction()
reactionsChatMessageReaction4.reactionType = 'like'

reactionsChatMessageReaction4.createdDateTime = DateTime('2018-10-21T02:34:40.3Z')

reactionsChatMessageReaction4User = ChatMessageReactionIdentitySet()
reactionsChatMessageReaction4User.application=null

reactionsChatMessageReaction4User.device=null

reactionsChatMessageReaction4UserUser = Identity()
reactionsChatMessageReaction4UserUser.id = '4c9041b7-449a-40f7-8855-56da239b9fd1'

reactionsChatMessageReaction4UserUser.displayName=null

additionalData = [
'userIdentityType' => 'aadUser', 
];
reactionsChatMessageReaction4UserUser.additionaldata(additionalData)



reactionsChatMessageReaction4User.user = reactionsChatMessageReaction4UserUser

reactionsChatMessageReaction4.user = reactionsChatMessageReaction4User

reactionsArray []= reactionsChatMessageReaction4;
reactionsChatMessageReaction5 = ChatMessageReaction()
reactionsChatMessageReaction5.reactionType = 'like'

reactionsChatMessageReaction5.createdDateTime = DateTime('2018-10-21T08:10:25.489Z')

reactionsChatMessageReaction5User = ChatMessageReactionIdentitySet()
reactionsChatMessageReaction5User.application=null

reactionsChatMessageReaction5User.device=null

reactionsChatMessageReaction5UserUser = Identity()
reactionsChatMessageReaction5UserUser.id = '03a02232-d8f5-4970-a77e-6e8c76ce7a4e'

reactionsChatMessageReaction5UserUser.displayName=null

additionalData = [
'userIdentityType' => 'aadUser', 
];
reactionsChatMessageReaction5UserUser.additionaldata(additionalData)



reactionsChatMessageReaction5User.user = reactionsChatMessageReaction5UserUser

reactionsChatMessageReaction5.user = reactionsChatMessageReaction5User

reactionsArray []= reactionsChatMessageReaction5;
reactionsChatMessageReaction6 = ChatMessageReaction()
reactionsChatMessageReaction6.reactionType = 'heart'

reactionsChatMessageReaction6.createdDateTime = DateTime('2018-10-21T08:10:31.489Z')

reactionsChatMessageReaction6User = ChatMessageReactionIdentitySet()
reactionsChatMessageReaction6User.application=null

reactionsChatMessageReaction6User.device=null

reactionsChatMessageReaction6UserUser = Identity()
reactionsChatMessageReaction6UserUser.id = '03a02232-d8f5-4970-a77e-6e8c76ce7a4e'

reactionsChatMessageReaction6UserUser.displayName=null

additionalData = [
'userIdentityType' => 'aadUser', 
];
reactionsChatMessageReaction6UserUser.additionaldata(additionalData)



reactionsChatMessageReaction6User.user = reactionsChatMessageReaction6UserUser

reactionsChatMessageReaction6.user = reactionsChatMessageReaction6User

reactionsArray []= reactionsChatMessageReaction6;
reactionsChatMessageReaction7 = ChatMessageReaction()
reactionsChatMessageReaction7.reactionType = 'sad'

reactionsChatMessageReaction7.createdDateTime = DateTime('2018-10-21T08:10:33.489Z')

reactionsChatMessageReaction7User = ChatMessageReactionIdentitySet()
reactionsChatMessageReaction7User.application=null

reactionsChatMessageReaction7User.device=null

reactionsChatMessageReaction7UserUser = Identity()
reactionsChatMessageReaction7UserUser.id = '03a02232-d8f5-4970-a77e-6e8c76ce7a4e'

reactionsChatMessageReaction7UserUser.displayName=null

additionalData = [
'userIdentityType' => 'aadUser', 
];
reactionsChatMessageReaction7UserUser.additionaldata(additionalData)



reactionsChatMessageReaction7User.user = reactionsChatMessageReaction7UserUser

reactionsChatMessageReaction7.user = reactionsChatMessageReaction7User

reactionsArray []= reactionsChatMessageReaction7;
reactionsChatMessageReaction8 = ChatMessageReaction()
reactionsChatMessageReaction8.reactionType = 'surprised'

reactionsChatMessageReaction8.createdDateTime = DateTime('2018-10-21T08:10:34.489Z')

reactionsChatMessageReaction8User = ChatMessageReactionIdentitySet()
reactionsChatMessageReaction8User.application=null

reactionsChatMessageReaction8User.device=null

reactionsChatMessageReaction8UserUser = Identity()
reactionsChatMessageReaction8UserUser.id = '03a02232-d8f5-4970-a77e-6e8c76ce7a4e'

reactionsChatMessageReaction8UserUser.displayName=null

additionalData = [
'userIdentityType' => 'aadUser', 
];
reactionsChatMessageReaction8UserUser.additionaldata(additionalData)



reactionsChatMessageReaction8User.user = reactionsChatMessageReaction8UserUser

reactionsChatMessageReaction8.user = reactionsChatMessageReaction8User

reactionsArray []= reactionsChatMessageReaction8;
request_body.reactions(reactionsArray)




request_configuration = ChatMessageRequestBuilderPatchRequestConfiguration(
)


result = await client.teams_by_id('team-id').channels_by_id('channel-id').messages_by_id('chatMessage-id').patch(request_body = request_body)


```