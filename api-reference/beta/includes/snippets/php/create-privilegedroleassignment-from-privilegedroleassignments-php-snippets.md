---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new PrivilegedRoleAssignment();


$requestRequestBody->setUserId('userId-value');
$requestRequestBody->setRoleId('roleId-value');
$result =  $graphClient->privilegedRoleAssignments()->post($requestRequestBody);


```