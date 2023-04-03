---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = ComplianceChange();
requestBody.set@odatatype('#microsoft.graph.windowsUpdates.complianceChange');

requestBody.setIsRevoked(true);



result = awaitclient.admin().windows().updates().updatePoliciesById('updatePolicy-id').complianceChangesById('complianceChange-id').patch(requestBody);


```