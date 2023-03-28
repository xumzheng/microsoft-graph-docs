---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new ItemPhone();
$requestBody.setDisplayName('Car Phone');

$requestBody.setNumber('+7 499 342 22 13');



$requestResult = $graphServiceClient.me().profile().phones().post($requestBody);


```