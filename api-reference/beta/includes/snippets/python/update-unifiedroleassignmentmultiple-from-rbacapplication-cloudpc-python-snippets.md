---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = UnifiedRoleAssignmentMultiple()
request_body.displayName = 'NewName'

request_body.description = 'A new roleAssignment'




result = await client.roleManagement.cloudPC.roleAssignments_by_id('unifiedRoleAssignmentMultiple-id').patch(request_body = request_body)


```