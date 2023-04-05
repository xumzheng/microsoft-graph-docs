---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ComplianceChange()
request_body.set@odatatype('#microsoft.graph.windowsUpdates.complianceChange')

request_body.setIsRevoked(true)



result = await client.admin.windows.updates.updatePolicies._by_id('updatePolicy-id').complianceChanges._by_id('complianceChange-id').patch(request_body)


```