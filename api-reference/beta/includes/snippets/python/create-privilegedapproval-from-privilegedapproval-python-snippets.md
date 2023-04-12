---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = PrivilegedApproval()
request_body.userId = 'userId-value'

request_body.roleId = 'roleId-value'

request_body.approvalType = 'approvalType-value'

request_body.ApprovalState(ApprovalState('approvalstate-value'))

request_body.approvalduration =  \DateInterval('datetime-value')




result = await client.privilegedApproval.post(request_body = request_body)


```