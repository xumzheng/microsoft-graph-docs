---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new ItemPhone();
$requestBody.setType(new PhoneType('other'));



$requestResult = $graphServiceClient.usersById('user-id').profile().phonesById('itemPhone-id').patch($requestBody);


```