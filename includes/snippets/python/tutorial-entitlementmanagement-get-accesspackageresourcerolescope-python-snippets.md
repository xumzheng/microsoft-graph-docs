---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AccessPackageResourceRoleScope()
accessPackageResourceRole = AccessPackageResourceRole()
accessPackageResourceRole.originId = 'Member_e93e24d1-2b65-4a6c-a1dd-654a12225487'

accessPackageResourceRole.displayName = 'Member'

accessPackageResourceRole.originSystem = 'AadGroup'

accessPackageResourceRoleAccessPackageResource = AccessPackageResource()
accessPackageResourceRoleAccessPackageResource.id = '4a1e21c5-8a76-4578-acb1-641160e076e8'

accessPackageResourceRoleAccessPackageResource.resourceType = 'Security Group'

accessPackageResourceRoleAccessPackageResource.originId = 'e93e24d1-2b65-4a6c-a1dd-654a12225487'

accessPackageResourceRoleAccessPackageResource.originSystem = 'AadGroup'


accessPackageResourceRole.accessPackageResource = accessPackageResourceRoleAccessPackageResource

request_body.accessPackageResourceRole = accessPackageResourceRole
accessPackageResourceScope = AccessPackageResourceScope()
accessPackageResourceScope.originId = 'e93e24d1-2b65-4a6c-a1dd-654a12225487'

accessPackageResourceScope.originSystem = 'AadGroup'


request_body.accessPackageResourceScope = accessPackageResourceScope



result = await client.identityGovernance.entitlementManagement.accessPackages_by_id('accessPackage-id').accessPackageResourceRoleScopes.post(request_body = request_body)


```