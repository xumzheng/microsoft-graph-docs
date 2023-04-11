---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = UserSource()
request_body.email = 'admin@M365x809305.onmicrosoft.com'

request_body.IncludedSources(SourceType('mailbox, site'))



request_configuration = UserSourcesRequestBuilderPostRequestConfiguration(
)


result = await client.security.cases.ediscoveryCases_by_id('ediscoveryCase-id').custodians_by_id('ediscoveryCustodian-id').userSources.post(request_body = request_body)


```