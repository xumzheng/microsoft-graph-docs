---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new UpdateSoftwarePostRequestBody();


$requestRequestBody->setSoftwareType(new TeamworkSoftwareType('teamsClient'));
$requestRequestBody->setSoftwareVersion('1.0.96.22');
$result =  $graphClient->teamwork()->devicesById('teamworkDevice-id')->updateSoftware()->post($requestRequestBody);


```