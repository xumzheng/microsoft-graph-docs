---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new Bookmark();


$requestRequestBody->setDescription('Book a fancy vacation in Tuscany or browse museums in Florence.');
$result =  $graphClient->search()->bookmarksById('bookmark-id')->patch($requestRequestBody);


```