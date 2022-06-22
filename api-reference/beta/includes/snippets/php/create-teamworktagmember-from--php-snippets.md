---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new TeamworkTagMember();


$requestRequestBody->setUserId('97f62344-57dc-409c-88ad-c4af14158ff5');
$result =  $graphClient->teamsById('team-id')->tagsById('teamworkTag-id')->members()->post($requestRequestBody);


```