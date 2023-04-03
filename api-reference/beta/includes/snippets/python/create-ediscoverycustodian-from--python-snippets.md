---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = EdiscoveryCustodian();
requestBody.setEmail('AdeleV@contoso.com');



result = awaitclient.security().cases().ediscoveryCasesById('ediscoveryCase-id').custodians().post(requestBody);


```