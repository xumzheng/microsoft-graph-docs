---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new CalendarGroup();


$requestRequestBody->setName('name-value');
$result =  $graphClient->me()->calendarGroupsById('calendarGroup-id')->patch($requestRequestBody);


```