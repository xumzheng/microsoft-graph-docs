---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new AccessPackageResourceRequest();
$requestBody.setCatalogId('beedadfe-01d5-4025-910b-84abb9369997');

$requestBody.setRequestType('AdminAdd');

$accessPackageResource = new AccessPackageResource();
$accessPackageResource.setOriginId('c6294667-7348-4f5a-be73-9d2c65f574f3');

$accessPackageResource.setOriginSystem('AadGroup');


$requestBody.setAccessPackageResource($accessPackageResource);


$requestResult = $graphServiceClient.identityGovernance().entitlementManagement().accessPackageResourceRequests().post($requestBody);


```