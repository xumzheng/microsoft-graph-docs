---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = PrivilegedApproval()
request_body.approvalstate(ApprovalState.ApprovalState-value('approvalstate.approvalstate-value'))

request_body.approver_reason = 'approverReason-value'




result = await client.privileged_approval.by_privileged_approval_id('privilegedApproval-id').patch(request_body = request_body)


```