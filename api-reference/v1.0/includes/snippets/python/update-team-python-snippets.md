---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new Team();
$memberSettings = new TeamMemberSettings();
$memberSettings.setAllowCreateUpdateChannels(true);


$requestBody.setMemberSettings($memberSettings);
$messagingSettings = new TeamMessagingSettings();
$messagingSettings.setAllowUserEditMessages(true);

$messagingSettings.setAllowUserDeleteMessages(true);


$requestBody.setMessagingSettings($messagingSettings);
$funSettings = new TeamFunSettings();
$funSettings.setAllowGiphy(true);

$funSettings.setGiphyContentRating(new GiphyRatingType('strict'));


$requestBody.setFunSettings($funSettings);


$requestResult = $graphServiceClient.teamsById('team-id').patch($requestBody);


```