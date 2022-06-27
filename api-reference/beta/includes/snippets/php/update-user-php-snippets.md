---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new User();


$requestRequestBody->setBusinessPhones(['+1 425 555 0109',]);
$requestRequestBody->setOfficeLocation('18/2111');
$result =  $graphClient->me()->patch($requestRequestBody);


```