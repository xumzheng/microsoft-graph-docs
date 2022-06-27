---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new TimeOffReason();


$requestRequestBody->setDisplayName('Vacation');
$requestRequestBody->setIconType(new TimeOffReasonIconType('plane'));
$requestRequestBody->setIsActive(True);
$result =  $graphClient->teamsById('team-id')->schedule()->timeOffReasons()->post($requestRequestBody);


```