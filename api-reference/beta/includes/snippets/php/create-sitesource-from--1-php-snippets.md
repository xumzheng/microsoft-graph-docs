---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new SiteSource();



$site = new Site();
$requestRequestBody->setSite($site);


$site->setWebUrl('https://contoso.sharepoint.com/sites/HumanResources');

$result =  $graphClient->compliance()->ediscovery()->casesById('case-id')->custodiansById('custodian-id')->siteSources()->post($requestRequestBody);


```