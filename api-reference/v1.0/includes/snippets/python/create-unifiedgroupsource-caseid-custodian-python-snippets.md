---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = UnifiedGroupSource()
group = Group()
group.mail = 'SOCTeam@M365x809305.onmicrosoft.com'


request_body.group = group
request_body.IncludedSources(SourceType('mailbox, site'))




result = await client.security.cases.ediscoveryCases_by_id('ediscoveryCase-id').custodians_by_id('ediscoveryCustodian-id').unifiedGroupSources.post(request_body = request_body)


```