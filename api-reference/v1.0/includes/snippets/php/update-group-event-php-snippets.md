---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new Event();



$location = new Location();
$requestRequestBody->setLocation($location);


$location->setDisplayName('Conf Room 2');

$result =  $graphClient->groupsById('group-id')->calendar()->eventsById('event-id')->patch($requestRequestBody);


```