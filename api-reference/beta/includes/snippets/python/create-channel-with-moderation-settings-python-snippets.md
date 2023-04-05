---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Channel()
request_body.setDisplayName('TestChannelModeration')

request_body.setDescription('Test channel moderation.')

request_body.setMembershipType(ChannelMembershipType('standard'))

moderationSettings = ChannelModerationSettings()
moderationSettings.setUserNewMessageRestriction(UserNewMessageRestriction('everyoneexceptguests'))

moderationSettings.setReplyRestriction(ReplyRestriction('everyone'))

moderationSettings.setAllowNewMessageFromBots(true)

moderationSettings.setAllowNewMessageFromConnectors(true)


request_body.setModerationSettings($moderationSettings)


result = await client.teams_by_id('team-id').channels.post(request_body)


```