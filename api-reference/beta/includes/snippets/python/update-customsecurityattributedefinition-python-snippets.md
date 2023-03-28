---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new CustomSecurityAttributeDefinition();
$requestBody.setDescription('Target completion date (YYYY/MM/DD)');



$requestResult = $graphServiceClient.directory().customSecurityAttributeDefinitionsById('customSecurityAttributeDefinition-id').patch($requestBody);


```