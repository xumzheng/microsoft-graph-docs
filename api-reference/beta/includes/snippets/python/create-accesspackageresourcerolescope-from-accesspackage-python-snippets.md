---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AccessPackageResourceRoleScope()
access_package_resource_role = AccessPackageResourceRole()
accessPackageResourceRole.originId = 'Member_b31fe1f1-3651-488f-bd9a-1711887fd4ca'

accessPackageResourceRole.displayName = 'Member'

accessPackageResourceRole.originSystem = 'AadGroup'

access_package_resource_role_access_package_resource = AccessPackageResource()
accessPackageResourceRoleAccessPackageResource.id = '1d08498d-72a1-403f-8511-6b1f875746a0'

accessPackageResourceRoleAccessPackageResource.resourceType = 'O365 Group'

accessPackageResourceRoleAccessPackageResource.originId = 'b31fe1f1-3651-488f-bd9a-1711887fd4ca'

accessPackageResourceRoleAccessPackageResource.originSystem = 'AadGroup'


accessPackageResourceRole.access_package_resource = accessPackageResourceRoleAccessPackageResource

request_body.access_package_resource_role = accessPackageResourceRole
access_package_resource_scope = AccessPackageResourceScope()
accessPackageResourceScope.originId = 'b31fe1f1-3651-488f-bd9a-1711887fd4ca'

accessPackageResourceScope.originSystem = 'AadGroup'


request_body.access_package_resource_scope = accessPackageResourceScope



result = await client.identityGovernance.entitlementManagement.accessPackages_by_id('accessPackage-id').accessPackageResourceRoleScopes.post(request_body = request_body)


```