---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ContactFolder();


$requestRequestBody->setDisplayName('Family');
$result =  $graphClient->me()->contactFoldersById('contactFolder-id')->childFolders()->post($requestRequestBody);


```