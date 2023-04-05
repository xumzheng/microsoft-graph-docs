---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AccessPackageResourceRoleScope()
accessPackageResourceRole = AccessPackageResourceRole()
accessPackageResourceRole.setOriginId('Member_b31fe1f1-3651-488f-bd9a-1711887fd4ca')

accessPackageResourceRole.setDisplayName('Member')

accessPackageResourceRole.setOriginSystem('AadGroup')

accessPackageResourceRoleAccessPackageResource = AccessPackageResource()
accessPackageResourceRoleAccessPackageResource.setId('1d08498d-72a1-403f-8511-6b1f875746a0')

accessPackageResourceRoleAccessPackageResource.setResourceType('O365 Group')

accessPackageResourceRoleAccessPackageResource.setOriginId('b31fe1f1-3651-488f-bd9a-1711887fd4ca')

accessPackageResourceRoleAccessPackageResource.setOriginSystem('AadGroup')


accessPackageResourceRole.setAccessPackageResource($accessPackageResourceRoleAccessPackageResource)

request_body.setAccessPackageResourceRole($accessPackageResourceRole)
accessPackageResourceScope = AccessPackageResourceScope()
accessPackageResourceScope.setOriginId('b31fe1f1-3651-488f-bd9a-1711887fd4ca')

accessPackageResourceScope.setOriginSystem('AadGroup')


request_body.setAccessPackageResourceScope($accessPackageResourceScope)


result = await client.identityGovernance.entitlementManagement.accessPackagesby_id('accessPackage-id').accessPackageResourceRoleScopes.post(request_body)


```