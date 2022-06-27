---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new GroupLifecyclePolicy();


$requestRequestBody->setGroupLifetimeInDays(180);
$requestRequestBody->setManagedGroupTypes('Selected');
$requestRequestBody->setAlternateNotificationEmails('admin@contoso.com');
$result =  $graphClient->groupLifecyclePoliciesById('groupLifecyclePolicy-id')->patch($requestRequestBody);


```