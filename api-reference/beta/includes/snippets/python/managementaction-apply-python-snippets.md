---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ApplyPostRequestBody()
request_body.tenantId = 'String'

request_body.tenantGroupId = 'String'

request_body.managementTemplateId = 'String'



request_configuration = ApplyRequestBuilderPostRequestConfiguration(
)


result = await client.tenantRelationships.managedTenants.managementActions_by_id('managementAction-id').managedTenantsapply.post(request_body = request_body)


```