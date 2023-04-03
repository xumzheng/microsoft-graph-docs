---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = EdiscoveryReviewSet();
requestBody.setDisplayName('My review set 2');



requestResult = graphServiceClient.security().cases().ediscoveryCasesById('ediscoveryCase-id').reviewSets().post(requestBody);


```