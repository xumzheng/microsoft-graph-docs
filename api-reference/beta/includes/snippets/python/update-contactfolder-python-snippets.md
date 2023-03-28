---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new ContactFolder();
$requestBody->setParentFolderId('parentFolderId-value');

$requestBody->setDisplayName('displayName-value');



$requestResult = $graphServiceClient->me()->contactFoldersById('contactFolder-id')->patch($requestBody);


```