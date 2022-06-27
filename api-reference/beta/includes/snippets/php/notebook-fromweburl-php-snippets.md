---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new WebUrlRequestBody();


$requestRequestBody->setWebUrl('webUrl value');
$result =  $graphClient->me()->onenote()->notebooks()->getNotebookFromWebUrl()->post($requestRequestBody);


```