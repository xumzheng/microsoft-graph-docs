---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Team()
request_body.setIsMembershipLimitedToOwners(true)

memberSettings = TeamMemberSettings()
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
discoverySettings = TeamDiscoverySettings()
discoverySettings.setShowInTeamsSearchAndSuggestions(true)


request_body.setDiscoverySettings($discoverySettings)


result = await client.teams_by_id('team-id').patch(request_body)


```