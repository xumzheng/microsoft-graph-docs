---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = EdiscoverySearch();
requestBody.setDisplayName('Teams search');



result = awaitclient.security().cases().ediscoveryCasesById('ediscoveryCase-id').searchesById('ediscoverySearch-id').patch(requestBody);


```