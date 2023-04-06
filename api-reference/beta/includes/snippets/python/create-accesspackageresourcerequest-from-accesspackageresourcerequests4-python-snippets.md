---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AccessPackageResourceRequest()
request_body.setCatalogId('beedadfe-01d5-4025-910b-84abb9369997')

request_body.setRequestType('AdminAdd')

accessPackageResource = AccessPackageResource()
accessPackageResource.setOriginId('c6294667-7348-4f5a-be73-9d2c65f574f3')

accessPackageResource.setOriginSystem('AadGroup')


request_body.setAccessPackageResource($accessPackageResource)


result = await client.identityGovernance.entitlementManagement.accessPackageResourceRequests.post(request_body, headers=)


```