---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = UserSource();
requestBody.setEmail('admin@M365x809305.onmicrosoft.com');

requestBody.setIncludedSources(SourceType('mailbox, site'));



result = awaitclient.security().cases().ediscoveryCasesById('ediscoveryCase-id').custodiansById('ediscoveryCustodian-id').userSources().post(requestBody);


```