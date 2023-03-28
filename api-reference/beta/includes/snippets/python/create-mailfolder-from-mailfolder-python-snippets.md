---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new MailFolder();
$requestBody->setDisplayName('displayName-value');

$requestBody->setIsHidden(true);



$requestResult = $graphServiceClient->me()->mailFoldersById('mailFolder-id')->childFolders()->post($requestBody);


```