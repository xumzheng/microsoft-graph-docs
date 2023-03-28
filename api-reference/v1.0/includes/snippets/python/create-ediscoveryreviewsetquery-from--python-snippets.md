---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new EdiscoveryReviewSetQuery();
$requestBody.setDisplayName('My Query 1');

$requestBody.setContentQuery('(Author=\"edison\")');



$requestResult = $graphServiceClient.security().cases().ediscoveryCasesById('ediscoveryCase-id').reviewSetsById('ediscoveryReviewSet-id').queries().post($requestBody);


```