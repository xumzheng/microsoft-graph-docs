---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = SiteSource()
site = Site()
site.webUrl = 'https://m365x809305.sharepoint.com/sites/Retail'


request_body.site = site


request_configuration = SiteSourcesRequestBuilderPostRequestConfiguration(
)


result = await client.security.cases.ediscoveryCases_by_id('ediscoveryCase-id').custodians_by_id('ediscoveryCustodian-id').siteSources.post(request_body = request_body)


```