---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new PrivilegedApproval();
$requestBody->setUserId('userId-value');

$requestBody->setRoleId('roleId-value');

$requestBody->setApprovalType('approvalType-value');

$requestBody->setApprovalState(new ApprovalState('approvalstate-value'));

$requestBody->setApprovalDuration(new \DateInterval('datetime-value'));



$requestResult = $graphServiceClient->privilegedApproval()->post($requestBody);


```