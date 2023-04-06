---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = DeletedItem()
additionalData = [
'userId' => '55ac777c-109e-4022-b58c-470c8fcb6892', 
'type' => 'Group', 
];
request_body.setAdditionalData(additionalData)




await client.directory.deletedItems_by_id('directoryObject-id').post(request_body, headers=)


```