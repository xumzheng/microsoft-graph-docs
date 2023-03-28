---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new CopyToDefaultContentLocationPostRequestBody();
$sourceFile = new ItemReference();
$sourceFileSharepointIds = new SharepointIds();
$sourceFileSharepointIds->setListId('e2ecf63b-b0fd-48f7-a54a-d8c15479e3b0');

$sourceFileSharepointIds->setListItemId('2');


$sourceFile->setSharepointIds($sourceFileSharepointIds);

$requestBody->setSourceFile($sourceFile);
$requestBody->setDestinationFileName('newname.txt');



$graphServiceClient->sitesById('site-id')->contentTypesById('contentType-id')->copyToDefaultContentLocation()->post($requestBody);


```