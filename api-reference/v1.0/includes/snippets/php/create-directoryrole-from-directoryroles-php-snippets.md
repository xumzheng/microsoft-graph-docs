---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new DirectoryRole();


$requestRequestBody->setRoleTemplateId('fe930be7-5e62-47db-91af-98c3a49a38b1');
$result =  $graphClient->directoryRoles()->post($requestRequestBody);


```