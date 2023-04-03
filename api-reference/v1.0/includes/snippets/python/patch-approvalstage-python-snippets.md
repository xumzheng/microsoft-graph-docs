---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = ApprovalStage();
requestBody.setReviewResult('Approve');

requestBody.setJustification('OK');



result = awaitclient.identityGovernance().entitlementManagement().accessPackageAssignmentApprovalsById('approval-id').stagesById('approvalStage-id').patch(requestBody);


```