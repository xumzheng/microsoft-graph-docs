---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = GovernanceRoleAssignmentRequest()
request_body.roleDefinitionId = '65bb4622-61f5-4f25-9d75-d0e20cf92019'

request_body.resourceId = 'e5e7d29d-5465-45ac-885f-4716a5ee74b5'

request_body.subjectId = '74765671-9ca4-40d7-9e36-2f4a570608a6'

request_body.assignmentState = 'Eligible'

request_body.type = 'AdminRemove'




result = await client.privilegedAccess_by_id('privilegedAccess-id').roleAssignmentRequests.post(request_body = request_body)


```