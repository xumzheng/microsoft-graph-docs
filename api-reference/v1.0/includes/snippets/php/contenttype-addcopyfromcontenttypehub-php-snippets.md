---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ContentTypeIdRequestBody();


$requestRequestBody->setContentTypeId('0x0101');
$result =  $graphClient->sitesById('site-id')->listsById('list-id')->contentTypes()->addCopyFromContentTypeHub()->post($requestRequestBody);


```