---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = PrivilegedApproval()
request_body.ApprovalState(ApprovalState('approvalstate-value'))

request_body.approverReason = 'approverReason-value'



request_configuration = PrivilegedApprovalRequestBuilderPatchRequestConfiguration(
)


result = await client.privilegedApproval_by_id('privilegedApproval-id').patch(request_body = request_body)


```