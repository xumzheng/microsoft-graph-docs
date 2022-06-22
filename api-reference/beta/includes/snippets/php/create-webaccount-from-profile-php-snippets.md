---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new WebAccount();


$requestRequestBody->setDescription('My Github contributions!');
$requestRequestBody->setUserId('innocenty.popov');

$service = new ServiceInformation();
$requestRequestBody->setService($service);


$service->setName('GitHub');
$service->setWebUrl('https://github.com');

$result =  $graphClient->me()->profile()->webAccounts()->post($requestRequestBody);


```