---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = Channel();
requestBody.setDisplayName('UpdateChannelModeration');

requestBody.setDescription('Update channel moderation.');

moderationSettings = ChannelModerationSettings();
moderationSettings.setUserNewMessageRestriction(UserNewMessageRestriction('moderators'));

moderationSettings.setReplyRestriction(ReplyRestriction('everyone'));

moderationSettings.setAllowNewMessageFromBots(true);

moderationSettings.setAllowNewMessageFromConnectors(true);


requestBody.setModerationSettings($moderationSettings);


result = awaitclient.teamsById('team-id').channelsById('channel-id').patch(requestBody);


```