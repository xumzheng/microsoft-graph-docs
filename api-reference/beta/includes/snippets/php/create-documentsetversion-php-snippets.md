---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new DocumentSetVersion();


$requestRequestBody->setComment('v1');
$requestRequestBody->setShouldCaptureMinorVersion(False);
$result =  $graphClient->sitesById('site-id')->listsById('list-id')->itemsById('listItem-id')->documentSetVersions()->post($requestRequestBody);


```