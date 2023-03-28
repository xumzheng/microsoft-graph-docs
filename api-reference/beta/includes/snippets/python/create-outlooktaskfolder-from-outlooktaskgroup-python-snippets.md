---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new OutlookTaskFolder();
$requestBody->setName('Cooking');



$requestResult = $graphServiceClient->me()->outlook()->taskGroupsById('outlookTaskGroup-id')->taskFolders()->post($requestBody);


```