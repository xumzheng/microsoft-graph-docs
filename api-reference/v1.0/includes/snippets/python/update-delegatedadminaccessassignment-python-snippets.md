---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = DelegatedAdminAccessAssignment();
accessDetails = DelegatedAdminAccessDetails();
unifiedRolesUnifiedRole1 = UnifiedRole();
unifiedRolesUnifiedRole1.setRoleDefinitionId('88d8e3e3-8f55-4a1e-953a-9b9898b8876b');


unifiedRolesArray []= unifiedRolesUnifiedRole1;
unifiedRolesUnifiedRole2 = UnifiedRole();
unifiedRolesUnifiedRole2.setRoleDefinitionId('44367163-eba1-44c3-98af-f5787879f96a');


unifiedRolesArray []= unifiedRolesUnifiedRole2;
unifiedRolesUnifiedRole3 = UnifiedRole();
unifiedRolesUnifiedRole3.setRoleDefinitionId('729827e3-9c14-49f7-bb1b-9608f156bbb8');


unifiedRolesArray []= unifiedRolesUnifiedRole3;
accessDetails.setUnifiedRoles(unifiedRolesArray);



requestBody.setAccessDetails($accessDetails);

request_config = DelegatedAdminAccessAssignmentRequestBuilderPatchRequestConfiguration();

headers = [
'If-Match' => 'W/"JyI0NzAwNjg0NS0wMDAwLTE5MDAtMDAwMC02MGY0Yjg4MzAwMDAiJw=="',
];

request_config.headers = headers;


result = awaitclient.tenantRelationships().delegatedAdminRelationshipsById('delegatedAdminRelationship-id').accessAssignmentsById('delegatedAdminAccessAssignment-id').patch(requestBody, request_config);


```