---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = SiteSource();
site = Site();
site.setWebUrl('https://contoso.sharepoint.com/sites/SecretSite');


request_body.setSite($site);


result = await client.compliance().ediscovery().casesById('case-id').legalHoldsById('legalHold-id').siteSources().post(request_body);


```