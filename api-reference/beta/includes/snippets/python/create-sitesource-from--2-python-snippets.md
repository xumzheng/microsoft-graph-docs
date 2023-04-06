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


result = await client.compliance.ediscovery.cases_by_id('case-id').legalHolds_by_id('legalHold-id').siteSources.post(request_body, headers=)


```