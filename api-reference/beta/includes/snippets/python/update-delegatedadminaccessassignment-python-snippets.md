---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = DelegatedAdminAccessAssignment()
accessDetails = DelegatedAdminAccessDetails()
unifiedRolesUnifiedRole1 = UnifiedRole()
unifiedRolesUnifiedRole1.roleDefinitionId = '88d8e3e3-8f55-4a1e-953a-9b9898b8876b'


unifiedRolesArray []= unifiedRolesUnifiedRole1;
unifiedRolesUnifiedRole2 = UnifiedRole()
unifiedRolesUnifiedRole2.roleDefinitionId = '44367163-eba1-44c3-98af-f5787879f96a'


unifiedRolesArray []= unifiedRolesUnifiedRole2;
unifiedRolesUnifiedRole3 = UnifiedRole()
unifiedRolesUnifiedRole3.roleDefinitionId = '729827e3-9c14-49f7-bb1b-9608f156bbb8'


unifiedRolesArray []= unifiedRolesUnifiedRole3;
accessDetails.unifiedroles(unifiedRolesArray)



request_body.accessDetails = accessDetails



result = await client.tenantRelationships.delegatedAdminRelationships_by_id('delegatedAdminRelationship-id').accessAssignments_by_id('delegatedAdminAccessAssignment-id').patch(request_body = request_body, request_configuration = request_configuration)


```