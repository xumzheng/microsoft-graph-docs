---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new AssociateWithHubSitesPostRequestBody();


$requestRequestBody->setHubSiteUrls( [
'https://graph.microsoft.com/v1.0/sites/{site-id}',],
$requestRequestBody->setPropagateToExistingLists(False);
$result =  $graphClient->sitesById('site-id')->contentTypesById('contentType-id')->associateWithHubSites()->post($requestRequestBody);


```