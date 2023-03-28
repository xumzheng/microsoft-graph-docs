---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new PersonInterest();
$requestBody.setCategories(['Sports', ]);

$requestBody.setDescription('World\'s greatest football club');

$requestBody.setDisplayName('Chelsea FC');

$requestBody.setWebUrl('https://www.chelseafc.com');



$requestResult = $graphServiceClient.me().profile().interests().post($requestBody);


```