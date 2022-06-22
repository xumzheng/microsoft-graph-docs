---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ScopedRoleMembership();


$requestRequestBody->setRoleId('roleId-value');

$roleMemberInfo = new Identity();
$requestRequestBody->setRoleMemberInfo($roleMemberInfo);


$roleMemberInfo->setId('id-value');

$result =  $graphClient->administrativeUnitsById('administrativeUnit-id')->scopedRoleMembers()->post($requestRequestBody);


```