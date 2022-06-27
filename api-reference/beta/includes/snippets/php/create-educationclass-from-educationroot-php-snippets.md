---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new EducationClass();


$requestRequestBody->setDescription('Health Level 1');
$requestRequestBody->setClassCode('Health 501');
$requestRequestBody->setDisplayName('Health 1');
$requestRequestBody->setExternalId('11019');
$requestRequestBody->setExternalName('Health Level 1');
$requestRequestBody->setExternalSource(new EducationExternalSource('sis'));
$requestRequestBody->setMailNickname('fineartschool.net');
$result =  $graphClient->education()->classes()->post($requestRequestBody);


```