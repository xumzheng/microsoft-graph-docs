---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = UnifiedGroupSource()
group = Group()
group.mail = 'SecretGroup@contoso.com'


request_body.group = group
request_body.IncludedSources(SourceType('mailbox, site'))



request_configuration = UnifiedGroupSourcesRequestBuilderPostRequestConfiguration(
)


result = await client.compliance.ediscovery.cases_by_id('case-id').custodians_by_id('custodian-id').unifiedGroupSources.post(request_body = request_body)


```