---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = UnifiedRoleEligibilityScheduleRequest()
request_body.action = 'adminRemove'

request_body.roleDefinitionId = '8424c6f0-a189-499e-bbd0-26c1753c96d4'

request_body.directoryScopeId = '/'

request_body.principalId = '071cc716-8147-4397-a5ba-b2105951cc0b'



request_configuration = RoleEligibilityScheduleRequestsRequestBuilderPostRequestConfiguration(
)


result = await client.roleManagement.directory.roleEligibilityScheduleRequests.post(request_body = request_body)


```