---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ContentType();


$requestRequestBody->setName('docSet');
$requestRequestBody->setDescription('custom docset');

$base = new ContentType();
$requestRequestBody->setBase($base);


$base->setName('Document Set');
$base->setId('0x0120D520');

$requestRequestBody->setGroup('Document Set Content Types');
$result =  $graphClient->sitesById('site-id')->contentTypes()->post($requestRequestBody);


```