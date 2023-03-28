---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new MailFolder();
$requestBody->setDisplayName('displayName-value');



$requestResult = $graphServiceClient->me()->mailFoldersById('mailFolder-id')->patch($requestBody);


```