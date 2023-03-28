---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new DelegatedPermissionClassification();
$requestBody.setPermissionId('e1fe6dd8-ba31-4d61-89e7-88639da4683d');

$requestBody.setPermissionName('User.Read');

$requestBody.setClassification(new PermissionClassificationType('low'));



$requestResult = $graphServiceClient.servicePrincipalsById('servicePrincipal-id').delegatedPermissionClassifications().post($requestBody);


```