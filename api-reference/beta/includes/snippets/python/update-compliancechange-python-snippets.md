---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ComplianceChange()
request_body.set@odatatype('#microsoft.graph.windowsUpdates.complianceChange')

request_body.setIsRevoked(true)



result = await client.admin.windows.updates.updatePolicies_by_id('updatePolicy-id').complianceChanges_by_id('complianceChange-id').patch(request_body, headers=)


```