---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = Channel();
requestBody.setDisplayName('TestChannelModeration');

requestBody.setDescription('Test channel moderation.');

requestBody.setMembershipType(ChannelMembershipType('standard'));

moderationSettings = ChannelModerationSettings();
moderationSettings.setUserNewMessageRestriction(UserNewMessageRestriction('everyoneexceptguests'));

moderationSettings.setReplyRestriction(ReplyRestriction('everyone'));

moderationSettings.setAllowNewMessageFromBots(true);

moderationSettings.setAllowNewMessageFromConnectors(true);


requestBody.setModerationSettings($moderationSettings);


result = await client.teamsById('team-id').channels().post(requestBody);


```