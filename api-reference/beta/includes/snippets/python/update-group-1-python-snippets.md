---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new Group();
$requestBody.setDescription('Contoso Life v2.0');

$requestBody.setDisplayName('Contoso Life Renewed');



$requestResult = $graphServiceClient.groupsById('group-id').patch($requestBody);


```