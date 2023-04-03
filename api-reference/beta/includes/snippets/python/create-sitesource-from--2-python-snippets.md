---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = SiteSource();
site = Site();
site.setWebUrl('https://contoso.sharepoint.com/sites/SecretSite');


requestBody.setSite($site);


result = awaitclient.compliance().ediscovery().casesById('case-id').legalHoldsById('legalHold-id').siteSources().post(requestBody);


```