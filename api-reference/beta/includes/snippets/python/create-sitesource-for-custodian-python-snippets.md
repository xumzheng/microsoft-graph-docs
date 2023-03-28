---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new SiteSource();
$site = new Site();
$site->setWebUrl('https://m365x809305.sharepoint.com/sites/Retail');


$requestBody->setSite($site);


$requestResult = $graphServiceClient->security()->cases()->ediscoveryCasesById('ediscoveryCase-id')->custodiansById('ediscoveryCustodian-id')->siteSources()->post($requestBody);


```