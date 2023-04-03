---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = SiteSource();
site = Site();
site.setWebUrl('https://contoso.sharepoint.com/sites/SecretSite');


requestBody.setSite($site);


requestResult = graphServiceClient.compliance().ediscovery().casesById('case-id').legalHoldsById('legalHold-id').siteSources().post(requestBody);


```