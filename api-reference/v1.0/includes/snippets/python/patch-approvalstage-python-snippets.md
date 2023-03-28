---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new ApprovalStage();
$requestBody->setReviewResult('Approve');

$requestBody->setJustification('OK');



$requestResult = $graphServiceClient->identityGovernance()->entitlementManagement()->accessPackageAssignmentApprovalsById('approval-id')->stagesById('approvalStage-id')->patch($requestBody);


```