---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new OutlookTaskFolder();


$requestRequestBody->setName('Cooking');
$result =  $graphClient->me()->outlook()->taskGroupsById('outlookTaskGroup-id')->taskFolders()->post($requestRequestBody);


```