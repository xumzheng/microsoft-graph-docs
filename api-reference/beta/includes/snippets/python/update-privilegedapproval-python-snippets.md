---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = PrivilegedApproval();
requestBody.setApprovalState(ApprovalState('approvalstate-value'));

requestBody.setApproverReason('approverReason-value');



result = await client.privilegedApprovalById('privilegedApproval-id').patch(requestBody);


```