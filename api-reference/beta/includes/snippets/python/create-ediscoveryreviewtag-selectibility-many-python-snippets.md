---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new EdiscoveryReviewTag();
$requestBody->setDisplayName('My tag API');

$requestBody->setDescription('Use Graph API to create tags');

$requestBody->setChildSelectability(new ChildSelectability('many'));



$requestResult = $graphServiceClient->security()->cases()->ediscoveryCasesById('ediscoveryCase-id')->tags()->post($requestBody);


```