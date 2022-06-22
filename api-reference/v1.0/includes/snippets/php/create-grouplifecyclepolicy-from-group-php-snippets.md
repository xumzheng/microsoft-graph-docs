---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new GroupLifecyclePolicy();


$requestRequestBody->setGroupLifetimeInDays(100);
$requestRequestBody->setManagedGroupTypes('Selected');
$requestRequestBody->setAlternateNotificationEmails('admin@contoso.com');
$result =  $graphClient->groupLifecyclePolicies()->post($requestRequestBody);


```