---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AccessPackageResourceRoleScope()
access_package_resource_role = AccessPackageResourceRole()
accessPackageResourceRole.originId = '4'

accessPackageResourceRole.originSystem = 'SharePointOnline'

access_package_resource_role_access_package_resource = AccessPackageResource()
accessPackageResourceRoleAccessPackageResource.id = '53c71803-a0a8-4777-aecc-075de8ee3991'


accessPackageResourceRole.access_package_resource = accessPackageResourceRoleAccessPackageResource

request_body.access_package_resource_role = accessPackageResourceRole
access_package_resource_scope = AccessPackageResourceScope()
accessPackageResourceScope.id = '5ae0ae7c-d0a5-42aa-ab37-1f15e9a61d33'

accessPackageResourceScope.originId = 'https://microsoft.sharepoint.com/portals/Community'

accessPackageResourceScope.originSystem = 'SharePointOnline'


request_body.access_package_resource_scope = accessPackageResourceScope



result = await client.identityGovernance.entitlementManagement.accessPackages_by_id('accessPackage-id').accessPackageResourceRoleScopes.post(request_body = request_body)


```