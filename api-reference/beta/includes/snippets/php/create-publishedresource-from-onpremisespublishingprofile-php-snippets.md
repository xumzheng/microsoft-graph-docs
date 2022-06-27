---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new PublishedResource();


$requestRequestBody->setDisplayName('New provisioning');
$requestRequestBody->setResourceName('domain1.contoso.com');
$result =  $graphClient->onPremisesPublishingProfilesById('onPremisesPublishingProfile-id')->publishedResources()->post($requestRequestBody);


```