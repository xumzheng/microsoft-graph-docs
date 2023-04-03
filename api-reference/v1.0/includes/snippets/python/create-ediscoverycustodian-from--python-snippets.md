---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = EdiscoveryCustodian();
requestBody.setEmail('AdeleV@contoso.com');



requestResult = graphServiceClient.security().cases().ediscoveryCasesById('ediscoveryCase-id').custodians().post(requestBody);


```