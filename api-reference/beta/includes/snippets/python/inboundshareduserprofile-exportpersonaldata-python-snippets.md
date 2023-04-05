---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ExportPersonalDataPostRequestBody()
request_body.setStorageLocation('MyStorageAccount')



await client.directory.inboundSharedUserProfilesById('inboundSharedUserProfile-userId').exportPersonalData.post(request_body)


```