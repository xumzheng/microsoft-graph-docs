---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new Team();



$memberSettings = new TeamMemberSettings();
$requestRequestBody->setMemberSettings($memberSettings);


$memberSettings->setAllowCreateUpdateChannels(True);


$messagingSettings = new TeamMessagingSettings();
$requestRequestBody->setMessagingSettings($messagingSettings);


$messagingSettings->setAllowUserEditMessages(True);
$messagingSettings->setAllowUserDeleteMessages(True);


$funSettings = new TeamFunSettings();
$requestRequestBody->setFunSettings($funSettings);


$funSettings->setAllowGiphy(True);
$funSettings->setGiphyContentRating(new GiphyRatingType('strict'));

$result =  $graphClient->teamsById('team-id')->patch($requestRequestBody);


```