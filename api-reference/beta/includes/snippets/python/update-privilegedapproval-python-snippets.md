---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new PrivilegedApproval();
$requestBody->setApprovalState(new ApprovalState('approvalstate-value'));

$requestBody->setApproverReason('approverReason-value');



$requestResult = $graphServiceClient->privilegedApprovalById('privilegedApproval-id')->patch($requestBody);


```