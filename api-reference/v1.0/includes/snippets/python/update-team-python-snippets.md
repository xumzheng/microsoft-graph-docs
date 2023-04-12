---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Team()
memberSettings = TeamMemberSettings()
memberSettings.allowCreateUpdateChannels = true


request_body.memberSettings = memberSettings
messagingSettings = TeamMessagingSettings()
messagingSettings.allowUserEditMessages = true

messagingSettings.allowUserDeleteMessages = true


request_body.messagingSettings = messagingSettings
funSettings = TeamFunSettings()
funSettings.allowGiphy = true

funSettings.GiphyContentRating(GiphyRatingType('strict'))


request_body.funSettings = funSettings



result = await client.teams_by_id('team-id').patch(request_body = request_body)


```