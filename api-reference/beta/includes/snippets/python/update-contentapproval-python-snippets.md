---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = ComplianceChange();
request_body.set@odatatype('#microsoft.graph.windowsUpdates.contentApproval');

request_body.setIsRevoked(true);



result = await client.admin().windows().updates().updatePoliciesById('updatePolicy-id').complianceChangesById('complianceChange-id').patch(request_body);


```