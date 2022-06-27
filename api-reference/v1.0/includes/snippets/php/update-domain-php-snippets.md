---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new Domain();


$requestRequestBody->setIsDefault(True);
$requestRequestBody->setSupportedServices(['Email','OfficeCommunicationsOnline',]);
$result =  $graphClient->domainsById('domain-id')->patch($requestRequestBody);


```