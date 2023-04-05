---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ExportPersonalDataPostRequestBody()
request_body.setStorageLocation('MyStorageAccount')



await client.directory_inboundSharedUserProfilesby_id('inboundSharedUserProfile-userId')_exportPersonalData.post(request_body)


```