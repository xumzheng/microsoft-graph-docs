---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new PrivilegedApproval();


$requestRequestBody->setUserId('userId-value');
$requestRequestBody->setRoleId('roleId-value');
$requestRequestBody->setApprovalType('approvalType-value');
$requestRequestBody->setApprovalState(new ApprovalState('approvalState-value'));
$requestRequestBody->setApprovalDuration('datetime-value');
$result =  $graphClient->privilegedApproval()->post($requestRequestBody);


```