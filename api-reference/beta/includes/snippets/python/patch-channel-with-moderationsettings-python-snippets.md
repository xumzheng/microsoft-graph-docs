---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Channel()
request_body.setDisplayName('UpdateChannelModeration')

request_body.setDescription('Update channel moderation.')

moderationSettings = ChannelModerationSettings()
moderationSettings.setUserNewMessageRestriction(UserNewMessageRestriction('moderators'))

moderationSettings.setReplyRestriction(ReplyRestriction('everyone'))

moderationSettings.setAllowNewMessageFromBots(true)

moderationSettings.setAllowNewMessageFromConnectors(true)


request_body.setModerationSettings($moderationSettings)

request_config = ChannelRequestBuilderPatchRequestConfiguration(
request_config = ChannelRequestBuilderPatchRequestConfiguration(query_params=)


result = await client.teams_by_id('team-id').channels_by_id('channel-id').patch(request_body, headers=)


```