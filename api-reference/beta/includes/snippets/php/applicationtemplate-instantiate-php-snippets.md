---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new DisplayNameRequestBody();


$requestRequestBody->setDisplayName('testProperties');
$result =  $graphClient->applicationTemplatesById('applicationTemplate-id')->instantiate()->post($requestRequestBody);


```