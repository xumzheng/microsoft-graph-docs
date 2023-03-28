---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new AllowedValue();
$requestBody.setIsActive(false);



$requestResult = $graphServiceClient.directory().customSecurityAttributeDefinitionsById('customSecurityAttributeDefinition-id').allowedValuesById('allowedValue-id').patch($requestBody);


```