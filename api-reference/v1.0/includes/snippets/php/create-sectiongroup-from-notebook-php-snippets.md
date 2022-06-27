---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new SectionGroup();


$requestRequestBody->setDisplayName('Section group name');
$result =  $graphClient->me()->onenote()->notebooksById('notebook-id')->sectionGroups()->post($requestRequestBody);


```