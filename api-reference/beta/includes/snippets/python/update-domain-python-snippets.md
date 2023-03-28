---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new Domain();
$requestBody.setIsDefault(true);

$requestBody.setSupportedServices(['Email', 'OfficeCommunicationsOnline', ]);



$requestResult = $graphServiceClient.domainsById('domain-id').patch($requestBody);


```