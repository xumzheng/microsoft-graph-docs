---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new WorkPosition();
$requestBody.setIsCurrent(true);



$requestResult = $graphServiceClient.me().profile().positionsById('workPosition-id').patch($requestBody);


```