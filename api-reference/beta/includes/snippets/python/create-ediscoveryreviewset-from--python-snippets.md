---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = EdiscoveryReviewSet();
requestBody.setDisplayName('My review set 2');



result = awaitclient.security().cases().ediscoveryCasesById('ediscoveryCase-id').reviewSets().post(requestBody);


```