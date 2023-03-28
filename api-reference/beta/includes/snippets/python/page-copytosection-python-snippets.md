---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new CopyToSectionPostRequestBody();
$requestBody.setId('id-value');

$requestBody.setGroupId('groupId-value');



$requestResult = $graphServiceClient.me().onenote().pagesById('onenotePage-id').copyToSection().post($requestBody);


```