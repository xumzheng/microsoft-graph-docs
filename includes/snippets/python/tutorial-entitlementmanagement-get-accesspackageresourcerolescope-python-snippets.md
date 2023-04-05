---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AccessPackageResourceRoleScope()
accessPackageResourceRole = AccessPackageResourceRole()
accessPackageResourceRole.setOriginId('Member_e93e24d1-2b65-4a6c-a1dd-654a12225487')

accessPackageResourceRole.setDisplayName('Member')

accessPackageResourceRole.setOriginSystem('AadGroup')

accessPackageResourceRoleAccessPackageResource = AccessPackageResource()
accessPackageResourceRoleAccessPackageResource.setId('4a1e21c5-8a76-4578-acb1-641160e076e8')

accessPackageResourceRoleAccessPackageResource.setResourceType('Security Group')

accessPackageResourceRoleAccessPackageResource.setOriginId('e93e24d1-2b65-4a6c-a1dd-654a12225487')

accessPackageResourceRoleAccessPackageResource.setOriginSystem('AadGroup')


accessPackageResourceRole.setAccessPackageResource($accessPackageResourceRoleAccessPackageResource)

request_body.setAccessPackageResourceRole($accessPackageResourceRole)
accessPackageResourceScope = AccessPackageResourceScope()
accessPackageResourceScope.setOriginId('e93e24d1-2b65-4a6c-a1dd-654a12225487')

accessPackageResourceScope.setOriginSystem('AadGroup')


request_body.setAccessPackageResourceScope($accessPackageResourceScope)


result = await client.identityGovernance_entitlementManagement_accessPackagesby_id('accessPackage-id')_accessPackageResourceRoleScopes.post(request_body)


```