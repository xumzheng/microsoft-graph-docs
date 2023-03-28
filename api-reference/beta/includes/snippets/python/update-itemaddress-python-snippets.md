---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new ItemAddress();
$requestBody.setAllowedAudiences(new AllowedAudiences('me'));

$requestBody.setDisplayName('Secret Hideout');



$requestResult = $graphServiceClient.usersById('user-id').profile().addressesById('itemAddress-id').patch($requestBody);


```