---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = UserSource()
request_body.setEmail('adelev@contoso.com')

request_body.setIncludedSources(SourceType('mailbox'))



result = await client.compliance.ediscovery.cases._by_id('case-id').legalHolds._by_id('legalHold-id').userSources.post(request_body)


```