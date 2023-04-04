---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = AccessPackageResourceRoleScope()
accessPackageResourceRole = AccessPackageResourceRole()
accessPackageResourceRole.setOriginId('4')

accessPackageResourceRole.setOriginSystem('SharePointOnline')

accessPackageResourceRoleAccessPackageResource = AccessPackageResource()
accessPackageResourceRoleAccessPackageResource.setId('53c71803-a0a8-4777-aecc-075de8ee3991')


accessPackageResourceRole.setAccessPackageResource($accessPackageResourceRoleAccessPackageResource)

request_body.setAccessPackageResourceRole($accessPackageResourceRole)
accessPackageResourceScope = AccessPackageResourceScope()
accessPackageResourceScope.setId('5ae0ae7c-d0a5-42aa-ab37-1f15e9a61d33')

accessPackageResourceScope.setOriginId('https://microsoft.sharepoint.com/portals/Community')

accessPackageResourceScope.setOriginSystem('SharePointOnline')


request_body.setAccessPackageResourceScope($accessPackageResourceScope)


result = await client.identityGovernance.entitlementManagement.accessPackagesById('accessPackage-id').accessPackageResourceRoleScopes.post(request_body)


```