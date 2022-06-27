---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new CopyToSectionPostRequestBody();


$requestRequestBody->setId('id-value');
$requestRequestBody->setGroupId('groupId-value');
$result =  $graphClient->me()->onenote()->pagesById('onenotePage-id')->copyToSection()->post($requestRequestBody);


```