---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = DeletedItem();
additionalData = [
'userId' => '55ac777c-109e-4022-b58c-470c8fcb6892', 
'type' => 'Group', 
];
requestBody.setAdditionalData(additionalData);




awaitclient.directory().deletedItemsById('directoryObject-id').post(requestBody);


```