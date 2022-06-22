---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new OnenoteSection();


$requestRequestBody->setDisplayName('Section name');
$result =  $graphClient->me()->onenote()->sectionGroupsById('sectionGroup-id')->sections()->post($requestRequestBody);


```