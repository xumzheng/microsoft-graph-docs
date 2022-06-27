---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new MailFolder();


$requestRequestBody->setDisplayName('Clutter');
$requestRequestBody->setIsHidden(True);
$result =  $graphClient->me()->mailFolders()->post($requestRequestBody);


```