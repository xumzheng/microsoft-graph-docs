---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ChangeDeploymentStatusPostRequestBody()
request_body.tenantGroupId = 'String'

request_body.tenantId = 'String'

request_body.managementActionId = 'String'

request_body.managementTemplateId = 'String'

request_body.status = 'String'



request_configuration = ChangeDeploymentStatusRequestBuilderPostRequestConfiguration(
)


result = await client.tenantRelationships.managedTenants.managementActionTenantDeploymentStatuses.managedTenantschangeDeploymentStatus.post(request_body = request_body)


```