---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = UserSource()
request_body.setEmail('admin@M365x809305.onmicrosoft.com')

request_body.setIncludedSources(SourceType('mailbox, site'))



result = await client.security.cases.ediscoveryCasesById('ediscoveryCase-id').legalHoldsById('ediscoveryHoldPolicy-id').userSources.post(request_body)


```