---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new OutlookTaskGroup();
$requestBody->setName('Personal Tasks');



$requestResult = $graphServiceClient->me()->outlook()->taskGroupsById('outlookTaskGroup-id')->patch($requestBody);


```