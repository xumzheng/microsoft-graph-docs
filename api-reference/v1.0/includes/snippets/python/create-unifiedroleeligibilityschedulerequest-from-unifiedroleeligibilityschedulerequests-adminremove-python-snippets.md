---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = UnifiedRoleEligibilityScheduleRequest()
request_body.setAction('adminRemove')

request_body.setRoleDefinitionId('8424c6f0-a189-499e-bbd0-26c1753c96d4')

request_body.setDirectoryScopeId('/')

request_body.setPrincipalId('071cc716-8147-4397-a5ba-b2105951cc0b')



result = await client.roleManagement.directory.roleEligibilityScheduleRequests.post(request_body, headers=)


```