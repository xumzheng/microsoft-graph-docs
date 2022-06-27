---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ContactFolder();


$requestRequestBody->setParentFolderId('parentFolderId-value');
$requestRequestBody->setDisplayName('displayName-value');
$result =  $graphClient->me()->contactFoldersById('contactFolder-id')->patch($requestRequestBody);


```