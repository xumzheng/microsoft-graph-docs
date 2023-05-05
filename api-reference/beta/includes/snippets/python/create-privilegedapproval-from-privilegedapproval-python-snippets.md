---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = PrivilegedApproval()
request_body.user_id = 'userId-value'

request_body.role_id = 'roleId-value'

request_body.approval_type = 'approvalType-value'

request_body.approvalstate(ApprovalState.ApprovalState-value('approvalstate.approvalstate-value'))

request_body.approvalduration =  \DateInterval('datetime-value')




result = await client.privileged_approval.post(request_body = request_body)


```