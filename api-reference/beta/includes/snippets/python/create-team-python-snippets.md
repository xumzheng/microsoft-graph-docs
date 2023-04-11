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
discoverySettings = TeamDiscoverySettings()
discoverySettings.showInTeamsSearchAndSuggestions = true


request_body.discoverySettings = discoverySettings


request_configuration = TeamRequestBuilderPutRequestConfiguration(
)


result = await client.groups_by_id('group-id').team.put(request_body = request_body)


```