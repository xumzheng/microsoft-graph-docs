---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ExportPersonalDataPostRequestBody()
request_body.setStorageLocation('storageLocation-value')



await client.usersById('user-id').exportPersonalData.post(request_body)


```