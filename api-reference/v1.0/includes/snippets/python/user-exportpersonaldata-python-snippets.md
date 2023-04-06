---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ExportPersonalDataPostRequestBody()
request_body.setStorageLocation('storageLocation-value')



await client.users_by_id('user-id').exportPersonalData.post(request_body, headers=)


```