---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Channel()
request_body.displayName = 'TestChannelModeration'

request_body.description = 'Test channel moderation.'

request_body.MembershipType(ChannelMembershipType('standard'))

moderation_settings = ChannelModerationSettings()
moderationSettings.UserNewMessageRestriction(UserNewMessageRestriction('everyoneexceptguests'))

moderationSettings.ReplyRestriction(ReplyRestriction('everyone'))

moderationSettings.allow_new_message_from_bots = True

moderationSettings.allow_new_message_from_connectors = True


request_body.moderation_settings = moderationSettings



result = await client.teams_by_id('team-id').channels.post(request_body = request_body)


```