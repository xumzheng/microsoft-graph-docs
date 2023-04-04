---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = DelegatedAdminAccessAssignment()
accessContainer = DelegatedAdminAccessContainer()
accessContainer.setAccessContainerId('869713c9-0b28-4d08-8949-ae07ae1bf528')

accessContainer.setAccessContainerType(DelegatedAdminAccessContainerType('securitygroup'))


request_body.setAccessContainer($accessContainer)
accessDetails = DelegatedAdminAccessDetails()
unifiedRolesUnifiedRole1 = UnifiedRole()
unifiedRolesUnifiedRole1.setRoleDefinitionId('29232cdf-9323-42fd-ade2-1d097af3e4de')


unifiedRolesArray []= unifiedRolesUnifiedRole1;
unifiedRolesUnifiedRole2 = UnifiedRole()
unifiedRolesUnifiedRole2.setRoleDefinitionId('f2ef992c-3afb-46b9-b7cf-a126ee74c451')


unifiedRolesArray []= unifiedRolesUnifiedRole2;
unifiedRolesUnifiedRole3 = UnifiedRole()
unifiedRolesUnifiedRole3.setRoleDefinitionId('729827e3-9c14-49f7-bb1b-9608f156bbb8')


unifiedRolesArray []= unifiedRolesUnifiedRole3;
unifiedRolesUnifiedRole4 = UnifiedRole()
unifiedRolesUnifiedRole4.setRoleDefinitionId('3a2c62db-5318-420d-8d74-23affee5d9d5')


unifiedRolesArray []= unifiedRolesUnifiedRole4;
accessDetails.setUnifiedRoles(unifiedRolesArray)



request_body.setAccessDetails($accessDetails)


result = await client.tenantRelationships.delegatedAdminRelationshipsById('delegatedAdminRelationship-id').accessAssignments.post(request_body)


```