---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new CopyToDefaultContentLocationPostRequestBody();



$sourceFile = new ItemReference();
$requestRequestBody->setSourceFile($sourceFile);



$sharepointIds = new SharepointIds();
$sourceFile->setSharepointIds($sharepointIds);


$sharepointIds->setListId('e2ecf63b-b0fd-48f7-a54a-d8c15479e3b0');
$sharepointIds->setListItemId('2');


$requestRequestBody->setDestinationFileName('newname.txt');
$result =  $graphClient->sitesById('site-id')->contentTypesById('contentType-id')->copyToDefaultContentLocation()->post($requestRequestBody);


```