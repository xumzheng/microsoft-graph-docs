---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = DelegatedAdminRelationship()
request_body.displayName = 'Updated Contoso admin relationship'

request_body.duration =  \DateInterval('P31D')

customer = DelegatedAdminRelationshipCustomerParticipant()
customer.tenantId = '52eaad04-13a2-4a2f-9ce8-93a294fadf36'


request_body.customer = customer
accessDetails = DelegatedAdminAccessDetails()
unifiedRolesUnifiedRole1 = UnifiedRole()
unifiedRolesUnifiedRole1.roleDefinitionId = '44367163-eba1-44c3-98af-f5787879f96a'


unifiedRolesArray []= unifiedRolesUnifiedRole1;
unifiedRolesUnifiedRole2 = UnifiedRole()
unifiedRolesUnifiedRole2.roleDefinitionId = '29232cdf-9323-42fd-ade2-1d097af3e4de'


unifiedRolesArray []= unifiedRolesUnifiedRole2;
unifiedRolesUnifiedRole3 = UnifiedRole()
unifiedRolesUnifiedRole3.roleDefinitionId = '69091246-20e8-4a56-aa4d-066075b2a7a8'


unifiedRolesArray []= unifiedRolesUnifiedRole3;
unifiedRolesUnifiedRole4 = UnifiedRole()
unifiedRolesUnifiedRole4.roleDefinitionId = '3a2c62db-5318-420d-8d74-23affee5d9d5'


unifiedRolesArray []= unifiedRolesUnifiedRole4;
accessDetails.unifiedroles(unifiedRolesArray)



request_body.accessDetails = accessDetails

headers = {
'If-Match' : "W/\"JyI0NzAwNjg0NS0wMDAwLTE5MDAtMDAwMC02MGY0Yjg4MzAwMDAiJw==\"",
}

)


result = await client.tenantRelationships.delegatedAdminRelationships_by_id('delegatedAdminRelationship-id').patch(request_body = request_body, request_configuration = request_configuration)


```