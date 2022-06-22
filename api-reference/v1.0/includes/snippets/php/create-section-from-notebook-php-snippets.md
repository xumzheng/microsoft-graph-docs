---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new OnenoteSection();


$requestRequestBody->setDisplayName('Section name');
$result =  $graphClient->me()->onenote()->notebooksById('notebook-id')->sections()->post($requestRequestBody);


```