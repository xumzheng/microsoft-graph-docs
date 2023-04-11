---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AccessPackageResourceRoleScope()
accessPackageResourceRole = AccessPackageResourceRole()
accessPackageResourceRole.originId = '4'

accessPackageResourceRole.originSystem = 'SharePointOnline'

accessPackageResourceRoleAccessPackageResource = AccessPackageResource()
accessPackageResourceRoleAccessPackageResource.id = '53c71803-a0a8-4777-aecc-075de8ee3991'


accessPackageResourceRole.accessPackageResource = accessPackageResourceRoleAccessPackageResource

request_body.accessPackageResourceRole = accessPackageResourceRole
accessPackageResourceScope = AccessPackageResourceScope()
accessPackageResourceScope.id = '5ae0ae7c-d0a5-42aa-ab37-1f15e9a61d33'

accessPackageResourceScope.originId = 'https://microsoft.sharepoint.com/portals/Community'

accessPackageResourceScope.originSystem = 'SharePointOnline'


request_body.accessPackageResourceScope = accessPackageResourceScope


request_configuration = AccessPackageResourceRoleScopesRequestBuilderPostRequestConfiguration(
)


result = await client.identityGovernance.entitlementManagement.accessPackages_by_id('accessPackage-id').accessPackageResourceRoleScopes.post(request_body = request_body)


```