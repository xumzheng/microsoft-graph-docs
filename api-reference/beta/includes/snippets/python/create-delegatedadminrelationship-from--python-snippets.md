---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = DelegatedAdminRelationship();
requestBody.setDisplayName('Contoso admin relationship');

$requestBody.setDuration( \DateInterval('P730D'));

customer = DelegatedAdminRelationshipCustomerParticipant();
customer.setTenantId('4b827261-d21f-4aa9-b7db-7fa1f56fb163');

customer.setDisplayName('Contoso subsidiary Inc');


requestBody.setCustomer($customer);
accessDetails = DelegatedAdminAccessDetails();
unifiedRolesUnifiedRole1 = UnifiedRole();
unifiedRolesUnifiedRole1.setRoleDefinitionId('29232cdf-9323-42fd-ade2-1d097af3e4de');


unifiedRolesArray []= unifiedRolesUnifiedRole1;
unifiedRolesUnifiedRole2 = UnifiedRole();
unifiedRolesUnifiedRole2.setRoleDefinitionId('3a2c62db-5318-420d-8d74-23affee5d9d5');


unifiedRolesArray []= unifiedRolesUnifiedRole2;
accessDetails.setUnifiedRoles(unifiedRolesArray);



requestBody.setAccessDetails($accessDetails);


result = awaitclient.tenantRelationships().delegatedAdminRelationships().post(requestBody);


```