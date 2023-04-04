---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = ApprovalStage();
request_body.setReviewResult('Approve');

request_body.setJustification('OK');



result = await client.identityGovernance.entitlementManagement.accessPackageAssignmentApprovalsById('approval-id').stagesById('approvalStage-id').patch(request_body);


```