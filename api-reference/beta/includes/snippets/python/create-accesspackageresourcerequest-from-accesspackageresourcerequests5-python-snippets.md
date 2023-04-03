---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = AccessPackageResourceRequest();
requestBody.setCatalogId('beedadfe-01d5-4025-910b-84abb9369997');

requestBody.setRequestType('AdminRemove');

accessPackageResource = AccessPackageResource();
accessPackageResource.setId('354078e5-dbce-4894-8af4-0ab274d41662');


requestBody.setAccessPackageResource($accessPackageResource);


requestResult = graphServiceClient.identityGovernance().entitlementManagement().accessPackageResourceRequests().post(requestBody);


```