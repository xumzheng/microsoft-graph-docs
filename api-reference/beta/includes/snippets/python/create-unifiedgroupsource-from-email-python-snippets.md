---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = UnifiedGroupSource()
group = Group()
group.setMail('SecretGroup@contoso.com')


request_body.setGroup($group)
request_body.setIncludedSources(SourceType('mailbox, site'))



result = await client.compliance.ediscovery.cases_by_id('case-id').custodians_by_id('custodian-id').unifiedGroupSources.post(request_body)


```