---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new SharePostRequestBody();


$requestRequestBody->setNotifyTeam(True);
$requestRequestBody->setStartDateTime(new DateTime("2018-10-08T00:00:00.000Z"));
$requestRequestBody->setEndDateTime(new DateTime("2018-10-15T00:00:00.000Z"));
$result =  $graphClient->teamsById('team-id')->schedule()->share()->post($requestRequestBody);


```