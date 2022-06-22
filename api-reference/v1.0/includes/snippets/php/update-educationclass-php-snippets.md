---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new EducationClass();


$requestRequestBody->setDescription('History - World History 1');
$requestRequestBody->setDisplayName('World History Level 1');
$result =  $graphClient->education()->classesById('educationClass-id')->patch($requestRequestBody);


```