---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = UnifiedRoleEligibilityScheduleRequest()
request_body.Action(UnifiedRoleScheduleRequestActions('adminremove'))

request_body.principalId = 'e77cbb23-0ff2-4e18-819c-690f58269752'

request_body.roleDefinitionId = 'fe930be7-5e62-47db-91af-98c3a49a38b1'

request_body.directoryScopeId = '/'




result = await client.roleManagement.directory.roleEligibilityScheduleRequests.post(request_body = request_body)


```