---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new PersonCertification();


$requestRequestBody->setIssuingAuthority('International Academy of Marketing Excellence');
$requestRequestBody->setIssuingCompany('International Academy of Marketing Excellence');
$result =  $graphClient->usersById('user-id')->profile()->certificationsById('personCertification-id')->patch($requestRequestBody);


```