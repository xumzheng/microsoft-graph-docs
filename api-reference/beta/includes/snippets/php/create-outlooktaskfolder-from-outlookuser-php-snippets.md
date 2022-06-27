---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new OutlookTaskFolder();


$requestRequestBody->setName('Volunteer');
$result =  $graphClient->me()->outlook()->taskFolders()->post($requestRequestBody);


```