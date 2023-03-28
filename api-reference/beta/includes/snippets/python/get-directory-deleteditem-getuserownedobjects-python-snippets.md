---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new GetUserOwnedObjectsPostRequestBody();
$requestBody.setUserId('55ac777c-109e-4022-b58c-470c8fcb6892');

$requestBody.setType('Group');



$requestResult = $graphServiceClient.directory().deletedItems().getUserOwnedObjects().post($requestBody);


```