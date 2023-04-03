---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = AccessPackageResourceRoleScope();
accessPackageResourceRole = AccessPackageResourceRole();
accessPackageResourceRole.setOriginId('Member_b31fe1f1-3651-488f-bd9a-1711887fd4ca');

accessPackageResourceRole.setDisplayName('Member');

accessPackageResourceRole.setOriginSystem('AadGroup');

accessPackageResourceRoleAccessPackageResource = AccessPackageResource();
accessPackageResourceRoleAccessPackageResource.setId('1d08498d-72a1-403f-8511-6b1f875746a0');

accessPackageResourceRoleAccessPackageResource.setResourceType('O365 Group');

accessPackageResourceRoleAccessPackageResource.setOriginId('b31fe1f1-3651-488f-bd9a-1711887fd4ca');

accessPackageResourceRoleAccessPackageResource.setOriginSystem('AadGroup');


accessPackageResourceRole.setAccessPackageResource($accessPackageResourceRoleAccessPackageResource);

requestBody.setAccessPackageResourceRole($accessPackageResourceRole);
accessPackageResourceScope = AccessPackageResourceScope();
accessPackageResourceScope.setOriginId('b31fe1f1-3651-488f-bd9a-1711887fd4ca');

accessPackageResourceScope.setOriginSystem('AadGroup');


requestBody.setAccessPackageResourceScope($accessPackageResourceScope);


requestResult = graphServiceClient.identityGovernance().entitlementManagement().accessPackagesById('accessPackage-id').accessPackageResourceRoleScopes().post(requestBody);


```