---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = EdiscoveryHoldPolicy();
requestBody.setDescription('updated description');



result = awaitclient.security().cases().ediscoveryCasesById('ediscoveryCase-id').legalHoldsById('ediscoveryHoldPolicy-id').patch(requestBody);


```