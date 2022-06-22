---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new SiteSource();



$site = new Site();
$requestRequestBody->setSite($site);


$site->setWebUrl('https://m365x809305.sharepoint.com/sites/Retail');

$result =  $graphClient->security()->cases()->ediscoveryCasesById('ediscoveryCase-id')->legalHoldsById('ediscoveryHoldPolicy-id')->siteSources()->post($requestRequestBody);


```