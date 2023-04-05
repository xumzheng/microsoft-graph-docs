---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = SiteSource()
site = Site()
site.setWebUrl('https://m365x809305.sharepoint.com/sites/Retail')


request_body.setSite($site)


result = await client.security_cases_ediscoveryCasesby_id('ediscoveryCase-id')_custodiansby_id('ediscoveryCustodian-id')_siteSources.post(request_body)


```