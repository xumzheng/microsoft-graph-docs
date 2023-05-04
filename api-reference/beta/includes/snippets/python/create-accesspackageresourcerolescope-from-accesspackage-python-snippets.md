---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Access_package_resource_role_scope()
access_package_resource_role = Access_package_resource_role()
access_package_resource_role.origin_id = 'Member_b31fe1f1-3651-488f-bd9a-1711887fd4ca'

access_package_resource_role.display_name = 'Member'

access_package_resource_role.origin_system = 'AadGroup'

access_package_resource_roleaccess_package_resource = Access_package_resource()
access_package_resource_roleaccess_package_resource.id = '1d08498d-72a1-403f-8511-6b1f875746a0'

access_package_resource_roleaccess_package_resource.resource_type = 'O365 Group'

access_package_resource_roleaccess_package_resource.origin_id = 'b31fe1f1-3651-488f-bd9a-1711887fd4ca'

access_package_resource_roleaccess_package_resource.origin_system = 'AadGroup'


access_package_resource_role.access_package_resource = access_package_resource_roleaccess_package_resource

request_body.access_package_resource_role = access_package_resource_role
access_package_resource_scope = Access_package_resource_scope()
access_package_resource_scope.origin_id = 'b31fe1f1-3651-488f-bd9a-1711887fd4ca'

access_package_resource_scope.origin_system = 'AadGroup'


request_body.access_package_resource_scope = access_package_resource_scope



result = await client.identity_governance.entitlement_management.acce_packages.by_acce_package_id('accessPackage-id').acces_package_resource_role_scopes.post(request_body = request_body)


```