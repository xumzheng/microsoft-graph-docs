---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new Group();


$requestRequestBody->setDisplayName('myGroup');
$result =  $graphClient->sitesById('site-id')->termStore()->groups()->post($requestRequestBody);


```