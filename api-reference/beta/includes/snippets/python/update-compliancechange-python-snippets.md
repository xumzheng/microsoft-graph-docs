---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ComplianceChange()
request_body.set@odatatype('#microsoft.graph.windowsUpdates.complianceChange')

request_body.setIsRevoked(true)



result = await client.admin.windows.updates.updatePoliciesby_id('updatePolicy-id').complianceChangesby_id('complianceChange-id').patch(request_body)


```