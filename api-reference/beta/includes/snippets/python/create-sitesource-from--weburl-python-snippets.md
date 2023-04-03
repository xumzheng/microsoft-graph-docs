---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = SiteSource();
site = Site();
site.setWebUrl('https://m365x809305.sharepoint.com/sites/Retail');


requestBody.setSite($site);


requestResult = graphServiceClient.security().cases().ediscoveryCasesById('ediscoveryCase-id').legalHoldsById('ediscoveryHoldPolicy-id').siteSources().post(requestBody);


```