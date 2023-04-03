---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = UserSource();
requestBody.setEmail('admin@M365x809305.onmicrosoft.com');

requestBody.setIncludedSources(SourceType('mailbox, site'));



requestResult = graphServiceClient.security().cases().ediscoveryCasesById('ediscoveryCase-id').legalHoldsById('ediscoveryHoldPolicy-id').userSources().post(requestBody);


```