---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Channel()
request_body.displayName = 'UpdateChannelModeration'

request_body.description = 'Update channel moderation.'

moderation_settings = ChannelModerationSettings()
moderationSettings.UserNewMessageRestriction(UserNewMessageRestriction('moderators'))

moderationSettings.ReplyRestriction(ReplyRestriction('everyone'))

moderationSettings.allow_new_message_from_bots = True

moderationSettings.allow_new_message_from_connectors = True


request_body.moderation_settings = moderationSettings



result = await client.teams_by_id('team-id').channels_by_id('channel-id').patch(request_body = request_body)


```