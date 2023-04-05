---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Team()
memberSettings = TeamMemberSettings()
memberSettings.setAllowCreatePrivateChannels(true)

memberSettings.setAllowCreateUpdateChannels(true)


request_body.setMemberSettings($memberSettings)
messagingSettings = TeamMessagingSettings()
messagingSettings.setAllowUserEditMessages(true)

messagingSettings.setAllowUserDeleteMessages(true)


request_body.setMessagingSettings($messagingSettings)
funSettings = TeamFunSettings()
funSettings.setAllowGiphy(true)

funSettings.setGiphyContentRating(GiphyRatingType('strict'))


request_body.setFunSettings($funSettings)


result = await client.groupsby_id('group-id').team.put(request_body)


```