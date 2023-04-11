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

fromUser.displayName = 'Sumit Gupta'

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


messageHistoryChatMessageHistoryItem1 = ChatMessageHistoryItem()
messageHistoryChatMessageHistoryItem1.modifiedDateTime = DateTime('2018-10-21T08:10:30.489Z')

messageHistoryChatMessageHistoryItem1.Actions(ChatMessageActions('reactionadded'))

messageHistoryChatMessageHistoryItem1Reaction = ChatMessageReaction()
messageHistoryChatMessageHistoryItem1Reaction.reactionType = 'angry'

messageHistoryChatMessageHistoryItem1ReactionUser = ChatMessageReactionIdentitySet()
messageHistoryChatMessageHistoryItem1ReactionUser.application=null

messageHistoryChatMessageHistoryItem1ReactionUser.device=null

messageHistoryChatMessageHistoryItem1ReactionUserUser = Identity()
messageHistoryChatMessageHistoryItem1ReactionUserUser.id = 'f1b66449-b46d-49b0-9c3c-53c10a5c818e'

messageHistoryChatMessageHistoryItem1ReactionUserUser.displayName=null

additionalData = [
'userIdentityType' => 'aadUser', 
];
messageHistoryChatMessageHistoryItem1ReactionUserUser.additionaldata(additionalData)



messageHistoryChatMessageHistoryItem1ReactionUser.user = messageHistoryChatMessageHistoryItem1ReactionUserUser

messageHistoryChatMessageHistoryItem1Reaction.user = messageHistoryChatMessageHistoryItem1ReactionUser

messageHistoryChatMessageHistoryItem1.reaction = messageHistoryChatMessageHistoryItem1Reaction

messageHistoryArray []= messageHistoryChatMessageHistoryItem1;
messageHistoryChatMessageHistoryItem2 = ChatMessageHistoryItem()
messageHistoryChatMessageHistoryItem2.modifiedDateTime = DateTime('2018-10-21T08:10:32.489Z')

messageHistoryChatMessageHistoryItem2.Actions(ChatMessageActions('reactionadded'))

messageHistoryChatMessageHistoryItem2Reaction = ChatMessageReaction()
messageHistoryChatMessageHistoryItem2Reaction.reactionType = 'laugh'

messageHistoryChatMessageHistoryItem2ReactionUser = ChatMessageReactionIdentitySet()
messageHistoryChatMessageHistoryItem2ReactionUser.application=null

messageHistoryChatMessageHistoryItem2ReactionUser.device=null

messageHistoryChatMessageHistoryItem2ReactionUserUser = Identity()
messageHistoryChatMessageHistoryItem2ReactionUserUser.id = '03a02232-d8f5-4970-a77e-6e8c76ce7a4e'

messageHistoryChatMessageHistoryItem2ReactionUserUser.displayName=null

additionalData = [
'userIdentityType' => 'aadUser', 
];
messageHistoryChatMessageHistoryItem2ReactionUserUser.additionaldata(additionalData)



messageHistoryChatMessageHistoryItem2ReactionUser.user = messageHistoryChatMessageHistoryItem2ReactionUserUser

messageHistoryChatMessageHistoryItem2Reaction.user = messageHistoryChatMessageHistoryItem2ReactionUser

messageHistoryChatMessageHistoryItem2.reaction = messageHistoryChatMessageHistoryItem2Reaction

messageHistoryArray []= messageHistoryChatMessageHistoryItem2;
messageHistoryChatMessageHistoryItem3 = ChatMessageHistoryItem()
messageHistoryChatMessageHistoryItem3.modifiedDateTime = DateTime('2018-10-21T02:17:14.67Z')

messageHistoryChatMessageHistoryItem3.Actions(ChatMessageActions('reactionadded'))

messageHistoryChatMessageHistoryItem3Reaction = ChatMessageReaction()
messageHistoryChatMessageHistoryItem3Reaction.reactionType = 'like'

messageHistoryChatMessageHistoryItem3ReactionUser = ChatMessageReactionIdentitySet()
messageHistoryChatMessageHistoryItem3ReactionUser.application=null

messageHistoryChatMessageHistoryItem3ReactionUser.device=null

messageHistoryChatMessageHistoryItem3ReactionUserUser = Identity()
messageHistoryChatMessageHistoryItem3ReactionUserUser.id = 'f1b66449-b46d-49b0-9c3c-53c10a5c818e'

messageHistoryChatMessageHistoryItem3ReactionUserUser.displayName=null

additionalData = [
'userIdentityType' => 'aadUser', 
];
messageHistoryChatMessageHistoryItem3ReactionUserUser.additionaldata(additionalData)



messageHistoryChatMessageHistoryItem3ReactionUser.user = messageHistoryChatMessageHistoryItem3ReactionUserUser

messageHistoryChatMessageHistoryItem3Reaction.user = messageHistoryChatMessageHistoryItem3ReactionUser

messageHistoryChatMessageHistoryItem3.reaction = messageHistoryChatMessageHistoryItem3Reaction

messageHistoryArray []= messageHistoryChatMessageHistoryItem3;
messageHistoryChatMessageHistoryItem4 = ChatMessageHistoryItem()
messageHistoryChatMessageHistoryItem4.modifiedDateTime = DateTime('2018-10-21T02:34:40.3Z')

messageHistoryChatMessageHistoryItem4.Actions(ChatMessageActions('reactionadded'))

messageHistoryChatMessageHistoryItem4Reaction = ChatMessageReaction()
messageHistoryChatMessageHistoryItem4Reaction.reactionType = 'like'

messageHistoryChatMessageHistoryItem4ReactionUser = ChatMessageReactionIdentitySet()
messageHistoryChatMessageHistoryItem4ReactionUser.application=null

messageHistoryChatMessageHistoryItem4ReactionUser.device=null

messageHistoryChatMessageHistoryItem4ReactionUserUser = Identity()
messageHistoryChatMessageHistoryItem4ReactionUserUser.id = '4c9041b7-449a-40f7-8855-56da239b9fd1'

messageHistoryChatMessageHistoryItem4ReactionUserUser.displayName=null

additionalData = [
'userIdentityType' => 'aadUser', 
];
messageHistoryChatMessageHistoryItem4ReactionUserUser.additionaldata(additionalData)



messageHistoryChatMessageHistoryItem4ReactionUser.user = messageHistoryChatMessageHistoryItem4ReactionUserUser

messageHistoryChatMessageHistoryItem4Reaction.user = messageHistoryChatMessageHistoryItem4ReactionUser

messageHistoryChatMessageHistoryItem4.reaction = messageHistoryChatMessageHistoryItem4Reaction

messageHistoryArray []= messageHistoryChatMessageHistoryItem4;
messageHistoryChatMessageHistoryItem5 = ChatMessageHistoryItem()
messageHistoryChatMessageHistoryItem5.modifiedDateTime = DateTime('2018-10-21T08:10:25.489Z')

messageHistoryChatMessageHistoryItem5.Actions(ChatMessageActions('reactionadded'))

messageHistoryChatMessageHistoryItem5Reaction = ChatMessageReaction()
messageHistoryChatMessageHistoryItem5Reaction.reactionType = 'like'

messageHistoryChatMessageHistoryItem5ReactionUser = ChatMessageReactionIdentitySet()
messageHistoryChatMessageHistoryItem5ReactionUser.application=null

messageHistoryChatMessageHistoryItem5ReactionUser.device=null

messageHistoryChatMessageHistoryItem5ReactionUserUser = Identity()
messageHistoryChatMessageHistoryItem5ReactionUserUser.id = '03a02232-d8f5-4970-a77e-6e8c76ce7a4e'

messageHistoryChatMessageHistoryItem5ReactionUserUser.displayName=null

additionalData = [
'userIdentityType' => 'aadUser', 
];
messageHistoryChatMessageHistoryItem5ReactionUserUser.additionaldata(additionalData)



messageHistoryChatMessageHistoryItem5ReactionUser.user = messageHistoryChatMessageHistoryItem5ReactionUserUser

messageHistoryChatMessageHistoryItem5Reaction.user = messageHistoryChatMessageHistoryItem5ReactionUser

messageHistoryChatMessageHistoryItem5.reaction = messageHistoryChatMessageHistoryItem5Reaction

messageHistoryArray []= messageHistoryChatMessageHistoryItem5;
messageHistoryChatMessageHistoryItem6 = ChatMessageHistoryItem()
messageHistoryChatMessageHistoryItem6.modifiedDateTime = DateTime('2018-10-21T08:10:31.489Z')

messageHistoryChatMessageHistoryItem6.Actions(ChatMessageActions('reactionadded'))

messageHistoryChatMessageHistoryItem6Reaction = ChatMessageReaction()
messageHistoryChatMessageHistoryItem6Reaction.reactionType = 'heart'

messageHistoryChatMessageHistoryItem6ReactionUser = ChatMessageReactionIdentitySet()
messageHistoryChatMessageHistoryItem6ReactionUser.application=null

messageHistoryChatMessageHistoryItem6ReactionUser.device=null

messageHistoryChatMessageHistoryItem6ReactionUserUser = Identity()
messageHistoryChatMessageHistoryItem6ReactionUserUser.id = '03a02232-d8f5-4970-a77e-6e8c76ce7a4e'

messageHistoryChatMessageHistoryItem6ReactionUserUser.displayName=null

additionalData = [
'userIdentityType' => 'aadUser', 
];
messageHistoryChatMessageHistoryItem6ReactionUserUser.additionaldata(additionalData)



messageHistoryChatMessageHistoryItem6ReactionUser.user = messageHistoryChatMessageHistoryItem6ReactionUserUser

messageHistoryChatMessageHistoryItem6Reaction.user = messageHistoryChatMessageHistoryItem6ReactionUser

messageHistoryChatMessageHistoryItem6.reaction = messageHistoryChatMessageHistoryItem6Reaction

messageHistoryArray []= messageHistoryChatMessageHistoryItem6;
messageHistoryChatMessageHistoryItem7 = ChatMessageHistoryItem()
messageHistoryChatMessageHistoryItem7.modifiedDateTime = DateTime('2018-10-21T08:10:33.489Z')

messageHistoryChatMessageHistoryItem7.Actions(ChatMessageActions('reactionadded'))

messageHistoryChatMessageHistoryItem7Reaction = ChatMessageReaction()
messageHistoryChatMessageHistoryItem7Reaction.reactionType = 'sad'

messageHistoryChatMessageHistoryItem7ReactionUser = ChatMessageReactionIdentitySet()
messageHistoryChatMessageHistoryItem7ReactionUser.application=null

messageHistoryChatMessageHistoryItem7ReactionUser.device=null

messageHistoryChatMessageHistoryItem7ReactionUserUser = Identity()
messageHistoryChatMessageHistoryItem7ReactionUserUser.id = '03a02232-d8f5-4970-a77e-6e8c76ce7a4e'

messageHistoryChatMessageHistoryItem7ReactionUserUser.displayName=null

additionalData = [
'userIdentityType' => 'aadUser', 
];
messageHistoryChatMessageHistoryItem7ReactionUserUser.additionaldata(additionalData)



messageHistoryChatMessageHistoryItem7ReactionUser.user = messageHistoryChatMessageHistoryItem7ReactionUserUser

messageHistoryChatMessageHistoryItem7Reaction.user = messageHistoryChatMessageHistoryItem7ReactionUser

messageHistoryChatMessageHistoryItem7.reaction = messageHistoryChatMessageHistoryItem7Reaction

messageHistoryArray []= messageHistoryChatMessageHistoryItem7;
messageHistoryChatMessageHistoryItem8 = ChatMessageHistoryItem()
messageHistoryChatMessageHistoryItem8.modifiedDateTime = DateTime('2018-10-21T08:10:34.489Z')

messageHistoryChatMessageHistoryItem8.Actions(ChatMessageActions('surprised'))

messageHistoryChatMessageHistoryItem8Reaction = ChatMessageReaction()
messageHistoryChatMessageHistoryItem8Reaction.reactionType = 'sad'

messageHistoryChatMessageHistoryItem8ReactionUser = ChatMessageReactionIdentitySet()
messageHistoryChatMessageHistoryItem8ReactionUser.application=null

messageHistoryChatMessageHistoryItem8ReactionUser.device=null

messageHistoryChatMessageHistoryItem8ReactionUserUser = Identity()
messageHistoryChatMessageHistoryItem8ReactionUserUser.id = '03a02232-d8f5-4970-a77e-6e8c76ce7a4e'

messageHistoryChatMessageHistoryItem8ReactionUserUser.displayName=null

additionalData = [
'userIdentityType' => 'aadUser', 
];
messageHistoryChatMessageHistoryItem8ReactionUserUser.additionaldata(additionalData)



messageHistoryChatMessageHistoryItem8ReactionUser.user = messageHistoryChatMessageHistoryItem8ReactionUserUser

messageHistoryChatMessageHistoryItem8Reaction.user = messageHistoryChatMessageHistoryItem8ReactionUser

messageHistoryChatMessageHistoryItem8.reaction = messageHistoryChatMessageHistoryItem8Reaction

messageHistoryArray []= messageHistoryChatMessageHistoryItem8;
request_body.messagehistory(messageHistoryArray)




request_configuration = ChatMessageRequestBuilderPatchRequestConfiguration(
)


result = await client.teams_by_id('team-id').channels_by_id('channel-id').messages_by_id('chatMessage-id').patch(request_body = request_body)


```