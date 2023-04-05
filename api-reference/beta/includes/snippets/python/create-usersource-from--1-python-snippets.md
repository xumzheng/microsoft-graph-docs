---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = UserSource()
request_body.setEmail('megan@contoso.com')

request_body.setIncludedSources(SourceType('mailbox, site'))



result = await client.compliance.ediscovery.cases._by_id('case-id').custodians._by_id('custodian-id').userSources.post(request_body)


```