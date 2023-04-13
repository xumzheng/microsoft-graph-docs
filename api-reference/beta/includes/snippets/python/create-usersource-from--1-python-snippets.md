---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = UserSource()
request_body.email = 'megan@contoso.com'

request_body.IncludedSources(SourceType('mailbox, site'))




result = await client.compliance.ediscovery.cases_by_id('case-id').custodians_by_id('custodian-id').userSources.post(request_body = request_body)


```