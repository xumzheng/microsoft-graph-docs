---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = PrivilegedApproval();
requestBody.setUserId('userId-value');

requestBody.setRoleId('roleId-value');

requestBody.setApprovalType('approvalType-value');

requestBody.setApprovalState(ApprovalState('approvalstate-value'));

$requestBody.setApprovalDuration( \DateInterval('datetime-value'));



requestResult = graphServiceClient.privilegedApproval().post(requestBody);


```