---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = TenantCustomizedInformation()
request_body.@odatatype = '#microsoft.graph.managedTenants.tenantCustomizedInformation'

request_body.tenantId = 'String'

contacts_tenant_contact_information1 = TenantContactInformation()
contactsTenantContactInformation1.@odatatype = 'microsoft.graph.managedTenants.tenantContactInformation'

contactsTenantContactInformation1.name = 'String'

contactsTenantContactInformation1.title = 'String'

contactsTenantContactInformation1.email = 'String'

contactsTenantContactInformation1.phone = 'String'

contactsTenantContactInformation1.notes = 'String'


contactsArray []= contactsTenantContactInformation1;
request_body.contacts(contactsArray)


request_body.website = 'String'




result = await client.tenantRelationships.managedTenants.tenantsCustomizedInformation_by_id('tenantCustomizedInformation-id').patch(request_body = request_body)


```