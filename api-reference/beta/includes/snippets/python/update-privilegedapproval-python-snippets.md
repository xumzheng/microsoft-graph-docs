---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = PrivilegedApproval()
request_body.setApprovalState(ApprovalState('approvalstate-value'))

request_body.setApproverReason('approverReason-value')



result = await client.privilegedApprovalby_id('privilegedApproval-id').patch(request_body)


```