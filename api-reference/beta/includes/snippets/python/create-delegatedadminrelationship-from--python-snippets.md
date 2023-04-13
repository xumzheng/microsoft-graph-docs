---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = DelegatedAdminRelationship()
request_body.displayName = 'Contoso admin relationship'

request_body.duration =  \DateInterval('P730D')

customer = DelegatedAdminRelationshipCustomerParticipant()
customer.tenantId = '4b827261-d21f-4aa9-b7db-7fa1f56fb163'

customer.displayName = 'Contoso subsidiary Inc'


request_body.customer = customer
access_details = DelegatedAdminAccessDetails()
unified_roles_unified_role1 = UnifiedRole()
unifiedRolesUnifiedRole1.roleDefinitionId = '29232cdf-9323-42fd-ade2-1d097af3e4de'


unifiedRolesArray []= unifiedRolesUnifiedRole1;
unified_roles_unified_role2 = UnifiedRole()
unifiedRolesUnifiedRole2.roleDefinitionId = '3a2c62db-5318-420d-8d74-23affee5d9d5'


unifiedRolesArray []= unifiedRolesUnifiedRole2;
accessDetails.unifiedroles(unifiedRolesArray)



request_body.access_details = accessDetails



result = await client.tenantRelationships.delegatedAdminRelationships.post(request_body = request_body)


```