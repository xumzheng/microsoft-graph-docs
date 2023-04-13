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

from_user = Identity()
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
attachments_chat_message_attachment1 = ChatMessageAttachment()
attachmentsChatMessageAttachment1.id = 'e8f78756199240b88448ae0fc6db112d'

attachmentsChatMessageAttachment1.contentType = 'application/vnd.microsoft.card.hero'

attachmentsChatMessageAttachment1.contentUrl=null

attachmentsChatMessageAttachment1.content = '{\r\n  \"title\": \"*title*\",\r\n  \"subtitle\": \"*subtitle*\",\r\n  \"text\": \"Have you found yourself scratching your head trying to figure these questions out? Frustrated trying to access some of the goodies unique to the Microsoft Teams platform?  Well, fear not, Bot Builder SDK Extension for Teams in .NET and Node flavors is here!  Just head on over to Nuget or NPM to download our tasty helpers, sure to speed up your prep time so you can spend more time maximizing the flavor of the bots you\'re cooking up.Here’s a small sample of some recipes to whet your appetite.\",\r\n  \"images\": [\r\n    {\r\n      \"url\": \"https://us-api.asm.skype.com/v1/objects/0-eus-d8-ced0c9567ee7b0b233b987bd32f9eacd/views/img_preview\"\r\n    }\r\n  ],\r\n  \"buttons\": [\r\n    {\r\n      \"type\": \"openUrl\",\r\n      \"image\": \"https://urlp.asm.skype.com/v1/url/content?url=https%3a%2f%2fcdn2.iconfinder.com%2fdata%2ficons%2fsocial-icons-33%2f128%2fTrello-128.png\",\r\n      \"title\": \"😃😃 click me 😃😃\",\r\n      \"value\": \"http://microsoft.com\"\r\n    },\r\n    {\r\n      \"type\": \"imback\",\r\n      \"title\": \"&i am back& <>= \\"\",\r\n      \"value\": \"&i am back& <>= \\"\"\r\n    },\r\n    {\r\n      \"type\": \"openUrl\",\r\n      \"title\": \"Open URL\",\r\n      \"value\": \"http://google.com\"\r\n    }\r\n  ]\r\n}'

attachmentsChatMessageAttachment1.name=null

attachmentsChatMessageAttachment1.thumbnailUrl=null


attachmentsArray []= attachmentsChatMessageAttachment1;
attachments_chat_message_attachment2 = ChatMessageAttachment()
attachmentsChatMessageAttachment2.id = '638464e32834471ea202007da60a5ae6'

attachmentsChatMessageAttachment2.contentType = 'application/vnd.microsoft.card.hero'

attachmentsChatMessageAttachment2.contentUrl=null

attachmentsChatMessageAttachment2.content = '{\r\n  \"title\": \"*title*\",\r\n  \"subtitle\": \"*subtitle*\",\r\n  \"text\": \"Have you found yourself scratching your head trying to figure these questions out? Frustrated trying to access some of the goodies unique to the Microsoft Teams platform?  Well, fear not, Bot Builder SDK Extension for Teams in .NET and Node flavors is here!  Just head on over to Nuget or NPM to download our tasty helpers, sure to speed up your prep time so you can spend more time maximizing the flavor of the bots you\'re cooking up.Here’s a small sample of some recipes to whet your appetite.\",\r\n  \"images\": [\r\n    {\r\n      \"url\": \"https://us-api.asm.skype.com/v1/objects/0-eus-d8-ced0c9567ee7b0b233b987bd32f9eacd/views/img_preview\"\r\n    }\r\n  ],\r\n  \"buttons\": [\r\n    {\r\n      \"type\": \"messageBack\",\r\n      \"title\": \"&message back& <>= \\"\",\r\n      \"text\": \"text = &message back& <>= \\"\",\r\n      \"displayText\": \"displayText = &message back& <>= \\"\",\r\n      \"value\": {\r\n        \"text\": \"some text 2\"\r\n      }\r\n    }\r\n  ]\r\n}'

attachmentsChatMessageAttachment2.name=null

attachmentsChatMessageAttachment2.thumbnailUrl=null


attachmentsArray []= attachmentsChatMessageAttachment2;
request_body.attachments(attachmentsArray)


request_body.Mentions([])

reactions_chat_message_reaction1 = ChatMessageReaction()
reactionsChatMessageReaction1.reactionType = 'angry'

reactionsChatMessageReaction1.createdDateTime = DateTime('2018-10-21T08:10:30.489Z')

reactions_chat_message_reaction1_user = ChatMessageReactionIdentitySet()
reactionsChatMessageReaction1User.application=null

reactionsChatMessageReaction1User.device=null

reactions_chat_message_reaction1_user_user = Identity()
reactionsChatMessageReaction1UserUser.id = 'f1b66449-b46d-49b0-9c3c-53c10a5c818e'

reactionsChatMessageReaction1UserUser.displayName=null

additionalData = [
'userIdentityType' => 'aadUser', 
];
reactionsChatMessageReaction1UserUser.additionaldata(additionalData)



reactionsChatMessageReaction1User.user = reactionsChatMessageReaction1UserUser

reactionsChatMessageReaction1.user = reactionsChatMessageReaction1User

reactionsArray []= reactionsChatMessageReaction1;
reactions_chat_message_reaction2 = ChatMessageReaction()
reactionsChatMessageReaction2.reactionType = 'laugh'

reactionsChatMessageReaction2.createdDateTime = DateTime('2018-10-21T08:10:32.489Z')

reactions_chat_message_reaction2_user = ChatMessageReactionIdentitySet()
reactionsChatMessageReaction2User.application=null

reactionsChatMessageReaction2User.device=null

reactions_chat_message_reaction2_user_user = Identity()
reactionsChatMessageReaction2UserUser.id = '03a02232-d8f5-4970-a77e-6e8c76ce7a4e'

reactionsChatMessageReaction2UserUser.displayName=null

additionalData = [
'userIdentityType' => 'aadUser', 
];
reactionsChatMessageReaction2UserUser.additionaldata(additionalData)



reactionsChatMessageReaction2User.user = reactionsChatMessageReaction2UserUser

reactionsChatMessageReaction2.user = reactionsChatMessageReaction2User

reactionsArray []= reactionsChatMessageReaction2;
reactions_chat_message_reaction3 = ChatMessageReaction()
reactionsChatMessageReaction3.reactionType = 'like'

reactionsChatMessageReaction3.createdDateTime = DateTime('2018-10-21T02:17:14.67Z')

reactions_chat_message_reaction3_user = ChatMessageReactionIdentitySet()
reactionsChatMessageReaction3User.application=null

reactionsChatMessageReaction3User.device=null

reactions_chat_message_reaction3_user_user = Identity()
reactionsChatMessageReaction3UserUser.id = 'f1b66449-b46d-49b0-9c3c-53c10a5c818e'

reactionsChatMessageReaction3UserUser.displayName=null

additionalData = [
'userIdentityType' => 'aadUser', 
];
reactionsChatMessageReaction3UserUser.additionaldata(additionalData)



reactionsChatMessageReaction3User.user = reactionsChatMessageReaction3UserUser

reactionsChatMessageReaction3.user = reactionsChatMessageReaction3User

reactionsArray []= reactionsChatMessageReaction3;
reactions_chat_message_reaction4 = ChatMessageReaction()
reactionsChatMessageReaction4.reactionType = 'like'

reactionsChatMessageReaction4.createdDateTime = DateTime('2018-10-21T02:34:40.3Z')

reactions_chat_message_reaction4_user = ChatMessageReactionIdentitySet()
reactionsChatMessageReaction4User.application=null

reactionsChatMessageReaction4User.device=null

reactions_chat_message_reaction4_user_user = Identity()
reactionsChatMessageReaction4UserUser.id = '4c9041b7-449a-40f7-8855-56da239b9fd1'

reactionsChatMessageReaction4UserUser.displayName=null

additionalData = [
'userIdentityType' => 'aadUser', 
];
reactionsChatMessageReaction4UserUser.additionaldata(additionalData)



reactionsChatMessageReaction4User.user = reactionsChatMessageReaction4UserUser

reactionsChatMessageReaction4.user = reactionsChatMessageReaction4User

reactionsArray []= reactionsChatMessageReaction4;
reactions_chat_message_reaction5 = ChatMessageReaction()
reactionsChatMessageReaction5.reactionType = 'like'

reactionsChatMessageReaction5.createdDateTime = DateTime('2018-10-21T08:10:25.489Z')

reactions_chat_message_reaction5_user = ChatMessageReactionIdentitySet()
reactionsChatMessageReaction5User.application=null

reactionsChatMessageReaction5User.device=null

reactions_chat_message_reaction5_user_user = Identity()
reactionsChatMessageReaction5UserUser.id = '03a02232-d8f5-4970-a77e-6e8c76ce7a4e'

reactionsChatMessageReaction5UserUser.displayName=null

additionalData = [
'userIdentityType' => 'aadUser', 
];
reactionsChatMessageReaction5UserUser.additionaldata(additionalData)



reactionsChatMessageReaction5User.user = reactionsChatMessageReaction5UserUser

reactionsChatMessageReaction5.user = reactionsChatMessageReaction5User

reactionsArray []= reactionsChatMessageReaction5;
reactions_chat_message_reaction6 = ChatMessageReaction()
reactionsChatMessageReaction6.reactionType = 'heart'

reactionsChatMessageReaction6.createdDateTime = DateTime('2018-10-21T08:10:31.489Z')

reactions_chat_message_reaction6_user = ChatMessageReactionIdentitySet()
reactionsChatMessageReaction6User.application=null

reactionsChatMessageReaction6User.device=null

reactions_chat_message_reaction6_user_user = Identity()
reactionsChatMessageReaction6UserUser.id = '03a02232-d8f5-4970-a77e-6e8c76ce7a4e'

reactionsChatMessageReaction6UserUser.displayName=null

additionalData = [
'userIdentityType' => 'aadUser', 
];
reactionsChatMessageReaction6UserUser.additionaldata(additionalData)



reactionsChatMessageReaction6User.user = reactionsChatMessageReaction6UserUser

reactionsChatMessageReaction6.user = reactionsChatMessageReaction6User

reactionsArray []= reactionsChatMessageReaction6;
reactions_chat_message_reaction7 = ChatMessageReaction()
reactionsChatMessageReaction7.reactionType = 'sad'

reactionsChatMessageReaction7.createdDateTime = DateTime('2018-10-21T08:10:33.489Z')

reactions_chat_message_reaction7_user = ChatMessageReactionIdentitySet()
reactionsChatMessageReaction7User.application=null

reactionsChatMessageReaction7User.device=null

reactions_chat_message_reaction7_user_user = Identity()
reactionsChatMessageReaction7UserUser.id = '03a02232-d8f5-4970-a77e-6e8c76ce7a4e'

reactionsChatMessageReaction7UserUser.displayName=null

additionalData = [
'userIdentityType' => 'aadUser', 
];
reactionsChatMessageReaction7UserUser.additionaldata(additionalData)



reactionsChatMessageReaction7User.user = reactionsChatMessageReaction7UserUser

reactionsChatMessageReaction7.user = reactionsChatMessageReaction7User

reactionsArray []= reactionsChatMessageReaction7;
reactions_chat_message_reaction8 = ChatMessageReaction()
reactionsChatMessageReaction8.reactionType = 'surprised'

reactionsChatMessageReaction8.createdDateTime = DateTime('2018-10-21T08:10:34.489Z')

reactions_chat_message_reaction8_user = ChatMessageReactionIdentitySet()
reactionsChatMessageReaction8User.application=null

reactionsChatMessageReaction8User.device=null

reactions_chat_message_reaction8_user_user = Identity()
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


message_history_chat_message_history_item1 = ChatMessageHistoryItem()
messageHistoryChatMessageHistoryItem1.modifiedDateTime = DateTime('2018-10-21T08:10:30.489Z')

messageHistoryChatMessageHistoryItem1.Actions(ChatMessageActions('reactionadded'))

message_history_chat_message_history_item1_reaction = ChatMessageReaction()
messageHistoryChatMessageHistoryItem1Reaction.reactionType = 'angry'

message_history_chat_message_history_item1_reaction_user = ChatMessageReactionIdentitySet()
messageHistoryChatMessageHistoryItem1ReactionUser.application=null

messageHistoryChatMessageHistoryItem1ReactionUser.device=null

message_history_chat_message_history_item1_reaction_user_user = Identity()
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
message_history_chat_message_history_item2 = ChatMessageHistoryItem()
messageHistoryChatMessageHistoryItem2.modifiedDateTime = DateTime('2018-10-21T08:10:32.489Z')

messageHistoryChatMessageHistoryItem2.Actions(ChatMessageActions('reactionadded'))

message_history_chat_message_history_item2_reaction = ChatMessageReaction()
messageHistoryChatMessageHistoryItem2Reaction.reactionType = 'laugh'

message_history_chat_message_history_item2_reaction_user = ChatMessageReactionIdentitySet()
messageHistoryChatMessageHistoryItem2ReactionUser.application=null

messageHistoryChatMessageHistoryItem2ReactionUser.device=null

message_history_chat_message_history_item2_reaction_user_user = Identity()
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
message_history_chat_message_history_item3 = ChatMessageHistoryItem()
messageHistoryChatMessageHistoryItem3.modifiedDateTime = DateTime('2018-10-21T02:17:14.67Z')

messageHistoryChatMessageHistoryItem3.Actions(ChatMessageActions('reactionadded'))

message_history_chat_message_history_item3_reaction = ChatMessageReaction()
messageHistoryChatMessageHistoryItem3Reaction.reactionType = 'like'

message_history_chat_message_history_item3_reaction_user = ChatMessageReactionIdentitySet()
messageHistoryChatMessageHistoryItem3ReactionUser.application=null

messageHistoryChatMessageHistoryItem3ReactionUser.device=null

message_history_chat_message_history_item3_reaction_user_user = Identity()
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
message_history_chat_message_history_item4 = ChatMessageHistoryItem()
messageHistoryChatMessageHistoryItem4.modifiedDateTime = DateTime('2018-10-21T02:34:40.3Z')

messageHistoryChatMessageHistoryItem4.Actions(ChatMessageActions('reactionadded'))

message_history_chat_message_history_item4_reaction = ChatMessageReaction()
messageHistoryChatMessageHistoryItem4Reaction.reactionType = 'like'

message_history_chat_message_history_item4_reaction_user = ChatMessageReactionIdentitySet()
messageHistoryChatMessageHistoryItem4ReactionUser.application=null

messageHistoryChatMessageHistoryItem4ReactionUser.device=null

message_history_chat_message_history_item4_reaction_user_user = Identity()
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
message_history_chat_message_history_item5 = ChatMessageHistoryItem()
messageHistoryChatMessageHistoryItem5.modifiedDateTime = DateTime('2018-10-21T08:10:25.489Z')

messageHistoryChatMessageHistoryItem5.Actions(ChatMessageActions('reactionadded'))

message_history_chat_message_history_item5_reaction = ChatMessageReaction()
messageHistoryChatMessageHistoryItem5Reaction.reactionType = 'like'

message_history_chat_message_history_item5_reaction_user = ChatMessageReactionIdentitySet()
messageHistoryChatMessageHistoryItem5ReactionUser.application=null

messageHistoryChatMessageHistoryItem5ReactionUser.device=null

message_history_chat_message_history_item5_reaction_user_user = Identity()
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
message_history_chat_message_history_item6 = ChatMessageHistoryItem()
messageHistoryChatMessageHistoryItem6.modifiedDateTime = DateTime('2018-10-21T08:10:31.489Z')

messageHistoryChatMessageHistoryItem6.Actions(ChatMessageActions('reactionadded'))

message_history_chat_message_history_item6_reaction = ChatMessageReaction()
messageHistoryChatMessageHistoryItem6Reaction.reactionType = 'heart'

message_history_chat_message_history_item6_reaction_user = ChatMessageReactionIdentitySet()
messageHistoryChatMessageHistoryItem6ReactionUser.application=null

messageHistoryChatMessageHistoryItem6ReactionUser.device=null

message_history_chat_message_history_item6_reaction_user_user = Identity()
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
message_history_chat_message_history_item7 = ChatMessageHistoryItem()
messageHistoryChatMessageHistoryItem7.modifiedDateTime = DateTime('2018-10-21T08:10:33.489Z')

messageHistoryChatMessageHistoryItem7.Actions(ChatMessageActions('reactionadded'))

message_history_chat_message_history_item7_reaction = ChatMessageReaction()
messageHistoryChatMessageHistoryItem7Reaction.reactionType = 'sad'

message_history_chat_message_history_item7_reaction_user = ChatMessageReactionIdentitySet()
messageHistoryChatMessageHistoryItem7ReactionUser.application=null

messageHistoryChatMessageHistoryItem7ReactionUser.device=null

message_history_chat_message_history_item7_reaction_user_user = Identity()
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
message_history_chat_message_history_item8 = ChatMessageHistoryItem()
messageHistoryChatMessageHistoryItem8.modifiedDateTime = DateTime('2018-10-21T08:10:34.489Z')

messageHistoryChatMessageHistoryItem8.Actions(ChatMessageActions('surprised'))

message_history_chat_message_history_item8_reaction = ChatMessageReaction()
messageHistoryChatMessageHistoryItem8Reaction.reactionType = 'sad'

message_history_chat_message_history_item8_reaction_user = ChatMessageReactionIdentitySet()
messageHistoryChatMessageHistoryItem8ReactionUser.application=null

messageHistoryChatMessageHistoryItem8ReactionUser.device=null

message_history_chat_message_history_item8_reaction_user_user = Identity()
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





result = await client.teams_by_id('team-id').channels_by_id('channel-id').messages_by_id('chatMessage-id').patch(request_body = request_body)


```