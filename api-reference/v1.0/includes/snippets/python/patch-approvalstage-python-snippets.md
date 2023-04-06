---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ApprovalStage()
request_body.setReviewResult('Approve')

request_body.setJustification('OK')



result = await client.identityGovernance.entitlementManagement.accessPackageAssignmentApprovals_by_id('approval-id').stages_by_id('approvalStage-id').patch(request_body, headers=)


```