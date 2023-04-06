---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = UserSource()
request_body.setEmail('admin@M365x809305.onmicrosoft.com')

request_body.setIncludedSources(SourceType('mailbox, site'))


request_config = UserSourcesRequestBuilderPostRequestConfiguration(
request_config = UserSourcesRequestBuilderPostRequestConfiguration(query_params=)


result = await client.security.cases.ediscoveryCases_by_id('ediscoveryCase-id').legalHolds_by_id('ediscoveryHoldPolicy-id').userSources.post(request_body, headers=)


```