---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new MailFolder();
$requestBody.setDisplayName('Clutter');

$requestBody.setIsHidden(true);



$requestResult = $graphServiceClient.me().mailFolders().post($requestBody);


```