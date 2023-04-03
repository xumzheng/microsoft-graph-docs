---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = Team();
memberSettings = TeamMemberSettings();
memberSettings.setAllowCreatePrivateChannels(true);

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


result = await client.groupsById('group-id').team().put(requestBody);


```