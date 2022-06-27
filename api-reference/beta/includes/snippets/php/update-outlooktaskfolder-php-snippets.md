---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new OutlookTaskFolder();


$requestRequestBody->setName('Charity work');
$result =  $graphClient->me()->outlook()->taskFoldersById('outlookTaskFolder-id')->patch($requestRequestBody);


```