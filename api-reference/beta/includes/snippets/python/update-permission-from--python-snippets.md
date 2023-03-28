---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new Permission();
$requestBody->setRoles(['read', ]);



$requestResult = $graphServiceClient->sitesById('site-id')->permissionsById('permission-id')->patch($requestBody);


```