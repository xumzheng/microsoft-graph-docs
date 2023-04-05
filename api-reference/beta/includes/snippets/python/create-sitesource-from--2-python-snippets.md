---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = SiteSource()
site = Site()
site.setWebUrl('https://contoso.sharepoint.com/sites/SecretSite')


request_body.setSite($site)


result = await client.compliance_ediscovery_casesby_id('case-id')_legalHoldsby_id('legalHold-id')_siteSources.post(request_body)


```