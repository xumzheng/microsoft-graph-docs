---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = PrivilegedApproval();
request_body.setUserId('userId-value');

request_body.setRoleId('roleId-value');

request_body.setApprovalType('approvalType-value');

request_body.setApprovalState(ApprovalState('approvalstate-value'));

$request_body.setApprovalDuration( \DateInterval('datetime-value'));



result = await client.privilegedApproval.post(request_body);


```