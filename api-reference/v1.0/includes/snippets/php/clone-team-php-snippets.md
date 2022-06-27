---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ClonePostRequestBody();


$requestRequestBody->setDisplayName('Library Assist');
$requestRequestBody->setDescription('Self help community for library');
$requestRequestBody->setMailNickname('libassist');
$requestRequestBody->setPartsToClone(new ClonableTeamParts('apps,tabs,settings,channels,members'));
$requestRequestBody->setVisibility(new TeamVisibilityType('public'));
$result =  $graphClient->teamsById('team-id')->clone()->post($requestRequestBody);


```