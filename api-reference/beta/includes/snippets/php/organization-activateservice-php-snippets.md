---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ActivateServicePostRequestBody();


$requestRequestBody->setSkuId('6fd2c87f-b296-42f0-b197-1e91e994b900');
$requestRequestBody->setServicePlanId('a23b959c-7ce8-4e57-9140-b90eb88a9e97');
$result =  $graphClient->organizationById('organization-id')->activateService()->post($requestRequestBody);


```