---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new EdiscoveryReviewTag();
$requestBody.setDisplayName('My tag API 2');

$requestBody.setDescription('Use Graph API to create tags (updated)');



$requestResult = $graphServiceClient.security().cases().ediscoveryCasesById('ediscoveryCase-id').tagsById('ediscoveryReviewTag-id').patch($requestBody);


```