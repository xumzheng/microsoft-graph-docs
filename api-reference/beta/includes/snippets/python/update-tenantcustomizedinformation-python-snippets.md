---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = TenantCustomizedInformation()
request_body.set@odatatype('#microsoft.graph.managedTenants.tenantCustomizedInformation')

request_body.setTenantId('String')

contactsTenantContactInformation1 = TenantContactInformation()
contactsTenantContactInformation1.set@odatatype('microsoft.graph.managedTenants.tenantContactInformation')

contactsTenantContactInformation1.setName('String')

contactsTenantContactInformation1.setTitle('String')

contactsTenantContactInformation1.setEmail('String')

contactsTenantContactInformation1.setPhone('String')

contactsTenantContactInformation1.setNotes('String')


contactsArray []= contactsTenantContactInformation1;
request_body.setContacts(contactsArray)


request_body.setWebsite('String')



result = await client.tenantRelationships.managedTenants.tenantsCustomizedInformation_by_id('tenantCustomizedInformation-id').patch(request_body)


```