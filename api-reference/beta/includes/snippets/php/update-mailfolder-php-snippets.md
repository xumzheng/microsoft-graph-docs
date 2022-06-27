---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new MailFolder();


$requestRequestBody->setDisplayName('displayName-value');
$result =  $graphClient->me()->mailFoldersById('mailFolder-id')->patch($requestRequestBody);


```