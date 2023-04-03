---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = Team();
requestBody.setIsMembershipLimitedToOwners(true);

memberSettings = TeamMemberSettings();
memberSettings.setAllowCreateUpdateChannels(true);


requestBody.setMemberSettings($memberSettings);
messagingSettings = TeamMessagingSettings();
messagingSettings.setAllowUserEditMessages(true);

messagingSettings.setAllowUserDeleteMessages(true);


requestBody.setMessagingSettings($messagingSettings);
funSettings = TeamFunSettings();
funSettings.setAllowGiphy(true);

funSettings.setGiphyContentRating(GiphyRatingType('strict'));


requestBody.setFunSettings($funSettings);
discoverySettings = TeamDiscoverySettings();
discoverySettings.setShowInTeamsSearchAndSuggestions(true);


requestBody.setDiscoverySettings($discoverySettings);


requestResult = graphServiceClient.teamsById('team-id').patch(requestBody);


```