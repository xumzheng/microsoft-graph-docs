---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new AttributeSet();
$requestBody.setDescription('Attributes for engineering team');

$requestBody.setMaxAttributesPerSet(20);



$requestResult = $graphServiceClient.directory().attributeSetsById('attributeSet-id').patch($requestBody);


```