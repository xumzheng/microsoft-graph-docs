---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new FieldValueSet();
$additionalData = [
'Color' => 'Fuchsia', 
'Quantity' => 934,
];
$requestBody->setAdditionalData($additionalData);




$requestResult = $graphServiceClient->sitesById('site-id')->listsById('list-id')->itemsById('listItem-id')->fields()->patch($requestBody);


```