---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new OutlookTaskFolder();
$requestBody.setName('Charity work');



$requestResult = $graphServiceClient.me().outlook().taskFoldersById('outlookTaskFolder-id').patch($requestBody);


```