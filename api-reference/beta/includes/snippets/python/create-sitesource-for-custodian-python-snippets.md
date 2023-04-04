---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = SiteSource()
site = Site()
site.setWebUrl('https://m365x809305.sharepoint.com/sites/Retail')


request_body.setSite($site)


result = await client.security.cases.ediscoveryCasesById('ediscoveryCase-id').custodiansById('ediscoveryCustodian-id').siteSources.post(request_body)


```