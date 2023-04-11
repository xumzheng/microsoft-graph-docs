---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AccessPackageResourceRoleScope()
accessPackageResourceRole = AccessPackageResourceRole()
accessPackageResourceRole.originId = 'Member_b31fe1f1-3651-488f-bd9a-1711887fd4ca'

accessPackageResourceRole.displayName = 'Member'

accessPackageResourceRole.originSystem = 'AadGroup'

accessPackageResourceRoleAccessPackageResource = AccessPackageResource()
accessPackageResourceRoleAccessPackageResource.id = '1d08498d-72a1-403f-8511-6b1f875746a0'

accessPackageResourceRoleAccessPackageResource.resourceType = 'O365 Group'

accessPackageResourceRoleAccessPackageResource.originId = 'b31fe1f1-3651-488f-bd9a-1711887fd4ca'

accessPackageResourceRoleAccessPackageResource.originSystem = 'AadGroup'


accessPackageResourceRole.accessPackageResource = accessPackageResourceRoleAccessPackageResource

request_body.accessPackageResourceRole = accessPackageResourceRole
accessPackageResourceScope = AccessPackageResourceScope()
accessPackageResourceScope.originId = 'b31fe1f1-3651-488f-bd9a-1711887fd4ca'

accessPackageResourceScope.originSystem = 'AadGroup'


request_body.accessPackageResourceScope = accessPackageResourceScope


request_configuration = AccessPackageResourceRoleScopesRequestBuilderPostRequestConfiguration(
)


result = await client.identityGovernance.entitlementManagement.accessPackages_by_id('accessPackage-id').accessPackageResourceRoleScopes.post(request_body = request_body)


```